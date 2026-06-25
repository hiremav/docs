# Source: https://knowledge.hiremav.com/zapier-app

1. [Knowledge Base](https://knowledge.hiremav.com/?hsLang=en)
2. [Integrations](https://knowledge.hiremav.com/integrations?hsLang=en)

# How does Mav's Zapier App Work?

## This guide describes how to integrate Mav with Zapier. Zapier is a web automation app that enables Mav users to connect to other online services like Salesforce, Hubspot, and thousands of others.

### Step 1 - Enable the Mav Zapier App in your Account.

[Click here](https://zapier.com/apps/mav/integrations) to enable the Mav Zapier app inside your Zapier account. At the time of writing our Zapier is private and at version 3.0.

### Step 2 -  Authenticate the Mav Zapier app with your Mav API Key.

Both Triggers and Actions will require you to authenticate your Zapier app to your Mav account. You can find your Mav API by [clicking here](https://hiremav.com/account_info) while logged into Mav.

Copy and Paste your API Key into the Zapier authentication window when asked in Step 3 and 4.

![Screen Shot 2021-11-30 at 4.59.34 PM](https://knowledge.hiremav.com/hs-fs/hubfs/Screen%20Shot%202021-11-30%20at%204.59.34%20PM.png?width=670&name=Screen%20Shot%202021-11-30%20at%204.59.34%20PM.png)

### Step 3 - Action Events (Inbound)

![Screen Shot 2021-11-30 at 4.58.05 PM](https://knowledge.hiremav.com/hs-fs/hubfs/Screen%20Shot%202021-11-30%20at%204.58.05%20PM.png?width=670&name=Screen%20Shot%202021-11-30%20at%204.58.05%20PM.png)

#### Run Playbook

Inside the "Run Playbook" Action Event you can provide the information on the lead.

#### ![Screen Shot 2021-11-30 at 5.00.53 PM](https://knowledge.hiremav.com/hs-fs/hubfs/Screen%20Shot%202021-11-30%20at%205.00.53%20PM.png?width=670&name=Screen%20Shot%202021-11-30%20at%205.00.53%20PM.png)

#### Stop Playbook

If you want to stop a running playbook you can do that with the "Stop Playbook" Action Event. This is as simple as passing the lead's phone number.

![Screen Shot 2021-11-30 at 5.01.06 PM](https://knowledge.hiremav.com/hs-fs/hubfs/Screen%20Shot%202021-11-30%20at%205.01.06%20PM.png?width=670&name=Screen%20Shot%202021-11-30%20at%205.01.06%20PM.png)

### Step 4 - Trigger Events (Outbound)

![Screen Shot 2021-11-30 at 5.01.18 PM](https://knowledge.hiremav.com/hs-fs/hubfs/Screen%20Shot%202021-11-30%20at%205.01.18%20PM.png?width=670&name=Screen%20Shot%202021-11-30%20at%205.01.18%20PM.png)

Mav fires triggers whenever a lead activity occurs. There are three trigger types:     

New Event - fires on conversational  and behavioral milestones

- started — Lead entered a playbook
- interested — Lead expressed interest
- message\_received — Inbound message received from lead
- stopped — Playbook stopped for this lead
- completed — Lead reached the end of the playbook
- reengagement\_sent — A re-engagement message was sent  
- qualified — Lead was marked as qualified                                                                 
- talk\_to\_human — Lead requested to speak with a human                                    
- talk\_to\_human\_spanish — Lead requested a Spanish-speaking human
- party\_line\_available — Party line call is available                                                                                              
- party\_line\_unavailable — Party line call could not be connected
- party\_line\_lead\_attempted — Party line call to lead was attempted
- party\_line\_lead\_unsuccessful — Party line call to lead did not connect
- party\_line\_lead\_answered — Lead answered the party line call                                                            
- party\_line\_rep\_attempted — Party line call to rep was attempted
- party\_line\_rep\_unsuccessful — Party line call to rep did not connect                                                
- party\_line\_lead\_initiated\_call — Lead initiated a party line call                                                            
- party\_line\_lead\_initiated\_call\_unsuccessful — Lead-initiated call did not connect

New Outcome — fires when a lead reaches a definitive result or disposition.

- unqualified — Lead was marked as unqualified
- not\_interested — Lead indicated no interest
- opted\_out — Lead opted out of messages
- undeliverable — Lead's phone number is undeliverable
- undeliverable\_rejected — Carrier rejected messages to this number
- **party\_line\_completed** — Party line call completed and successful