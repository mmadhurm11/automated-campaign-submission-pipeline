
# Automated Campaign Submission Filtering 

###  Problem
Student campaigns often faced **fake engagement**:
- Low-effort responses like "ok", "done", "nice".
- Multiple submissions from the same IP to meet minimum criteria.
- Manual filtering wasted time but still missed spam.
- This led to **low ROI** and fewer genuine active users.

---

###  Solution
I built a **2-stage automation pipeline** using **Make.com, Google Sheets, and Slack**:

1. **Quality Check** → filters spam/short comments, checks submission time ≥ 20 sec.  
2. **IP Uniqueness Check** → allows max 2 submissions per IP, else flagged.  
3. **Slack Alerts** → suspicious entries sent instantly to campaign team.  
4. **Clean Data Output** → valid vs flagged submissions stored in separate Google Sheets.

---

###  Workflow

- **Trigger:** Google Sheets (Watch new rows)  
- **Router 1:** Quality Check → pass/fail → store in Valid/Flagged sheets  
- **Router 2:** IP Check → prevent duplicates  
- **Slack Integration:** Real-time alerts for flagged entries  

---

###  Outcomes
-  Flagged **35%+ fake/invalid entries** automatically  
-  Reduced manual review workload by **~80%**  
-  Improved dataset **accuracy by 40%+**  
-  Delivered **trustworthy ROI measurement** for campaigns  

---

###  Repository Contents
- `data/campaign_submissions.xlsx` → Sample input dataset  
- `pipeline/grapevine_pipeline.json` → Exported Make.com workflow  
- `pipeline/pipeline_screenshot.png` → Visual of workflow  
- `docs/slide_deck.pdf` → Project presentation  
- `links.txt` → Link to the live Make.com pipeline  

---

###  Impact
This project showcases:
- **Automation for business ROI**  
- **Product-thinking approach** (cleaning user engagement signals)  
- **Scalable system design** using no-code tools  

---

###  Live Pipeline
 [Click here to view the live Make.com pipeline](https://eu2.make.com/2709273/scenarios/7360894/edit)
