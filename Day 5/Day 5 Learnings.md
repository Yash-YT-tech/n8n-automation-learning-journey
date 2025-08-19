# Day 5 – AI Recruitment Workflow (n8n)  

**What I Learned Today:**  

- 📋 **Form Setup**  
  - Built a form called *Team* for hackathon team members.  
  - Fields included: **Name, Experience, Language** (Python / HTML / CSS).  
  - This form collects all candidate info in a clean format.  

- 🗄️ **Airtable Connection**  
  - **Step 1:** Save candidate details into Airtable.  
  - **Step 2:** Update the same record with a rating based on language.  
  - Ratings were simple: Python ⭐5, CSS ⭐4, HTML ⭐3.  

- 🔀 **Switch Logic**  
  - The workflow checks the candidate’s **Language field**.  
  - Depending on the value, it applies the right rating.  
  - Green lines in n8n show which path is active.  

- 🤖 **AI Candidate Review**  
  - Used *Google Gemini Chat Model* as the “recruiter.”  
  - AI looks at: **Name, Experience, Language, Rating**.  
  - It then gives a **short opinion**: is this candidate worth considering or not?  

- 📝 **Final Record Update**  
  - The AI’s review is saved back into Airtable in the “Review” field.  
  - Same record gets updated throughout the workflow, so everything stays connected.  

- ⚙️ **Technical Learnings**  
  - Learned how to reference nodes (e.g., `$('Python Ratings').item.json.id`).  
  - Switch conditions need exact matches (case-sensitive).  
  - AI prompt works better with clear structure and placeholders (`{{ $json.fields.Name }}`).  

- 🌍 **Why This Is Useful**  
  - Automates the full candidate screening process.  
  - Combines fixed rules (ratings) with flexible AI analysis.  
  - Makes hiring faster and more consistent.  

- 🚀 **Extra Learnings**  
  - Same record can be created → updated → reviewed step by step.  
  - Branching logic makes the workflow flexible but still joins back later.  
  - AI isn’t just automating — it’s helping with real decisions.  

---

**📝 Final Takeaway:**  
Day 5 felt like a **big step forward**.  

I now know how to link forms, conditions, Airtable, and AI together.

Instead of just storing data, I can build a system that acts like a **smart recruiter** — it saves time, keeps things fair, and gives clear recommendations.  

---

## 🗂 Project Files
Click to view the files directly:    
✅ [Day 5 Workflow](./day5-workflow-code.json) 

✅ [Day 5 Workflow Screenshot](./day5-screenshot.png)

✅ [Day 5 Final Result](./day-result.png)




---

**Resources:**  
- 📺 Playlist: [AI Agents Masterclass](https://youtube.com/playlist?list=PLwdhOAfEpxTaHqf_o0waIy-EPz0PWEvFh&si=Jd125zWc1zOaKy-n)  
- ▶️ Day 5 Video: [Recruitment Workflow with AI](https://youtu.be/EHbAA8aERYc?si=ooijekdNfxQroml1)  





