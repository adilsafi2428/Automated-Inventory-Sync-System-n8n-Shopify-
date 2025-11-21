Automated Inventory Synchronization System (n8n & Shopify)
      This project delivers a bulletproof, two-way automated solution that eliminates manual errors and stockouts by flawlessly syncing live Shopify inventory with a central Google Sheets planning hub. It's built for scalability and reliability.
🎯 Key Design & Business ValuePrincipleValue
PropositionZero Error
TolerancePrevents Overselling!
Implements checks to block critical mistakes like Negative Stock entry.
Time SavingsEliminates manual, repetitive inventory checks. The system handles all scheduled syncs and event-based alerts automatically.
       Future-ProofModular and Scalable architecture ensures the system works just as efficiently with 5 products as it does with 5,000.🚀 Workflow Breakdown: The Engine of Automation
       The system operates on two distinct, interconnected n8n workflows
       🟢 Workflow A: Master Data Sync (The READ Operation)This workflow runs hourly to establish the single source of truth in your planning sheet.
       ComponentWhy It Matters (Value)Data StandardisationGuarantees 9 required data fields are present and standardized, ready for analysis and reporting.Location ID AccuracyDynamically fetches the correct Shopify Location ID (a common integration challenge) for every single variant.
       Proactive AlertingImplements the Low Stock Check logic to notify managers the moment restock is needed.2. 
       ✍️ Workflow B: Inventory Update & Alert (The WRITE Operation)This workflow runs instantly (event-driven) whenever a manual change is made in the Google Sheet.FunctionOutput ValueReal-Time UpdatePushes corrected quantities from the sheet instantly back to the live Shopify inventory—completing the two-way loop.Critical Safety CheckThe Negative Stock Check immediately triggers a high-priority alert to investigate system integrity failures.EfficiencyEnsures your live store always reflects the most up-to-date and verified stock count from your planning hub.
       📦 Repository FilesFile NameDescriptionREADME.mdThis project summary document.
       Workflow_A_Sync.jsonn8n export file for the Master Data Sync workflow.
       Workflow_B_Update.jsonn8n export file for the Inventory Update workflow.
       Sample_Google_Sheet.xlsxTemplate showing all required column headers for replication.
       🎥 Project DemoWatch the system in action: see a stock change instantly trigger an update on the live Shopify store!Link to Live Demo Video: [INSERT YOUR YOUTUBE/VIMEO LINK HERE]
