# Source: https://knowledge.hiremav.com/how-to-import-leads-via-csv-

1. [Knowledge Base](https://knowledge.hiremav.com/?hsLang=en)
2. [Lead Delivery](https://knowledge.hiremav.com/lead-delivery?hsLang=en)

# How to import Leads via CSV     

## Upload your list of leads directly into Mav

Mav's CSV import lets you upload a list of auto or home insurance leads directly into a playbook. This guide walks you through the full process, from preparing your file to tracking the import once it's running.

#### **What you'll need**

Before you begin, make sure you have:                                                                                 

- A CSV file containing your auto or home insurance leads                                                             
 
- The playbook you'd like these leads assigned to
 
- Confirmation that **every lead in the file** has given written or electronic consent (TCPA) to be contacted via automated SMS and voice calls                                                                                         
 

If you'd like a head start on formatting your file, you can download a pre-formatted template in Step 1.

####  **Step 1: Choose insurance type and playbook**

1. Navigate to **Settings → Imports** and click **New Import**.
 
2. Select the insurance type for your file: **Auto** or **Home**.
 
3. _(Optional)_  Click the **Auto** or **Home** template link to download a CSV with all supported column headers pre-filled. This is the easiest way to ensure your file matches our expected format.                                              
 
4. Choose the **playbook** you want these leads assigned to. Only playbooks that match the selected insurance type will be available.                                                                                                           
 
5.  Toggle the **TCPA Consent** switch to confirm that all leads in the file have provided proper consent. This step is required and cannot be skipped.                                                                                       
 
6. Click **Continue**. 
 

#### **Step 2: Upload your file and map columns**                                                                             

1. Click the file picker and select your CSV.
2. Once uploaded, Mav reads the column headers and displays a mapping table. Each of your columns will be auto-matched to a corresponding Mav field where possible (for example, a column named "Cell Phone" will be suggested as **Phone**).
3. Review each row in the mapping table:
 1. Confirm the suggested mapping is correct, or select a different field from the dropdown.
 2. For any column you don't want to import, select **Skip this column**.
4. At minimum, **one column must be mapped to Phone** — the import cannot proceed without it.
5. Click **Continue** when your mapping is complete. 

#### **Step 3: Preview and confirm**                                                                                          

1. Review the preview panel, which shows:
 
 1. The total number of leads detected in your file
 
 2. A preview of the first lead, formatted exactly as it will appear in Mav
 
2. If everything looks correct, click **Start Import**. If not, use the **Back** button to adjust your mapping.               
 

#### **Daily limits and scheduling**                                                                                           

To protect deliverability and pacing, imports are capped at **500 leads per account, per day**.

If your file contains 500 rows or fewer and you haven't imported earlier today, all leads will be processed immediately. If your file exceeds the daily limit, the remaining leads are automatically deferred and released the following business morning.

This continues day by day until the entire file has been processed - no further action is needed from you.

#### **Tracking the status of an import**                                           

After starting an import, you'll be taken to its details page. Here you can monitor:

- **Status**: New, importing, deferred, finished, or failed
 
- **Progress bar**: Shows how many rows have been processed
 
- **Import stats: C**ounts of successful imports, duplicates, rows missing a phone number, and any row-level errors      
 

You can return to this page any time from **Settings → Imports**. If an import fails, a **Retry** button will appear, which resumes from where it left off rather than restarting from the beginning.                                             

#### **How imported leads appear in Mav**                                           

Every lead brought in through this tool is tagged with the source **"Manual Import – YYYY-MM-DD"** (using the date of the import). This makes it easy to distinguish imported leads from leads coming in through your live integrations when filtering or reporting.                                                                                                

\---

If you run into trouble with a particular file or column mapping, reach out to support@hiremav.com 

Was this article helpful?

Yes No

### Related articles

- [How do Playbook Alerts work?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3p-N25j6MV3lXXbN6MK-lF69CG0W84S5Qh2nBFD4W35W3Ks2LQS4hW5S_Wct1PTpWDW8Bwq_X1SL3ndW6R2MPq9h4MC2W3x3CM66x704fW6M6_CL5zknQ5W6pvxbp6g5HgHN4NBk7T6M79hW2DqFVQ2GK9vWVqmT3p8qZztHW3ZQ5-D97VhcLW48Bdvf8yCnfGW7rcXjZ6RwyrnW82TY6g8f6vRpW8fN5cw1M8fgzW1ys0Zr473X7wW9k7H1g56q-V8N79QhSbs1pvGW4MGtTx6bGM3bW71fFVJ6XXzBjW3GNmLD1bJ4X2d_jrmY04)
- [How does Mav's Ricochet 360 Integration Work?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/JkM2-6qcW6N1vHY6lZ3nlV-T4PB2qGqm4W3lJhFV93zMNnW8JrPnd1ZsHTKW8Cj0d02lP6hGW58cnbQ2WhRlgW5SYLt27c96v3VF55sc4BQJztW55K-7h7F4Zn5VQXP9L2Yyph3W5fmzhP5hZXkVW799DCL6M5C6-W894CkR8cJZNlVQSvPr6htx6_N4kLC9Hg4WDhW1JKnW12m6DWRW8Z15cr7xp_xDW1BGByL8Sv6svW7MB8s875Gtp1W1LV3mj3TPjVdW2NPdLp4XJCPzN6Q51L_pGG_sW7w0NH89brTtjf6fhRc604)
- [Understanding Texting Hours in Mav](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3lCW6zF55725X3pfN7CLVYrRQFm9W6JFyFb4q6cY4W20x-GV2fmNF8W8K5p6M7Rf0tzW5bRsNZ2qlDW2W2Jbmh97VQYnwW9lTK7-1Nk859W389LzG2xx8LyVDhCNT33S3TtN2S6chd6qtwGW1MfgYC7pTbktW5xYrrg4cq3RLW93spsY887f5JVZlQCQ8LYxbYW5xzgK_2RXtCJW1qwZ1540l5cXVLgVrZ68QJv8W7l25ws7_q35sW8h99Ly6sjSW0W3T-FG13d44YwW48ZkdY8VRnZ9W8X72nr5BkJDKW4zpPvW1Wnc7yf91ZSKW04)
- [Party Lines Completed - Feature Reference](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3nRW5dYNbj3fqMD0W917ndC8GyhqPN7lP3fQct9R-W4CJJhy6PxflfW8fvnpR3tdyTxW2mgmCW3hPnx-W7sPrwC9cLzDqW7LvtqW2CttsPW1sry3q5wyfZ-W13GMq9178fVbW4dcVrm3Hf9CLW1y94Cn86G087W3YQ4JB7v400sW4Tsf0t5Fv7H2W3tyXjH1QsB5hW5HBS5M5sNP3TW7_ntnS54jd_1W5Vmx2f5Dw5GvW20HdwS8nQQNcW7ZhGZP5BxZx-W52LP1Z7MGTzrW1HLXQm72BBgnW1kjr1m2PtSQ5W4n11KZ65g23_f88djgR04)
- [How do I set a schedule for my Party Line live transfers?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jll2-6qcW7Y8-PT6lZ3kyVKh2dy1KBWn8W1prlR12vs38NW8yXZxx6yJzSGW76tGY68ZKkg6VRFpW443657XW7XZ9Xb8NZz-lW2jZhMM4l_nS1V9c4Nc3V0TfbW3kQMTf6H3ZPHW6dpfzS4PXFt2W3LFjvB6GJqKHW7Z0N2k94ynzRW4RZ-J_88DJJ_W1QBV9D6MQ5p-W2GQWLx2hD12LW7MMbQ22KxtgyVvgjLB3z_bb3W8PY_-08sGv0qW1KJb5b8_5nlzW98py3N4kZjfMVdJdRf6FbXgKW2Syh2t7-YBGMN78V2skhxn99W7gN6p24T5m2wW6hTJFv59L5XpW4D7-923V_dNzf3NLGJT04)