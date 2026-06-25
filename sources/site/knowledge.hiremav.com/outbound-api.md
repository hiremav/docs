# Source: https://knowledge.hiremav.com/outbound-api

1. [Knowledge Base](https://knowledge.hiremav.com/?hsLang=en)
2. [API](https://knowledge.hiremav.com/api?hsLang=en)

# Outbound API

## Mav’s outbound API consists of subscribing to either event or outcome activity. Activity subscriptions are optional. You can choose to subscribe to one, many or all of the available activities (events and outcomes) your playbook supports.

Mav’s outbound API consists of subscribing to either event or outcome activity via webhook URL.

Activity subscriptions are optional. You can choose to subscribe to one, many or all of the available activities (events and outcomes) your playbook supports.

**Event** activities are available across all playbooks and they include the following:

- **started** — when Mav sends out the first message to the lead
- **double\_opted\_in** — when a lead expresses positive intent and opts-in
- **interested** — when a lead expresses positive intent. Note: this is usually called at the same time as **double\_opted\_in.**
- **stopped** — when a playbook is stopped (either manually or during an opt-out)
- **completed** — when a playbook has reached an outcome
- **reengagement\_sent** — when Mav sends a smart re-engagement to a lead
- **party\_line\_lead\_attempted** — when Mav attempts to call the lead for a party line
- **party\_line\_lead\_unsuccessful** — when a lead doesn't confirm they would like to be connected
- **party\_line\_lead\_answered** — when the lead confirms they would like to be connected to the Rep
- **party\_line\_rep\_attempted** — when Mav attempts to call the rep for a party line
- **party\_line\_rep\_unsuccessful** — when Mav is unable to join the lead and rep for a party line
- **party\_line\_lead\_initiated\_call -** when a lead calls into your Mav number
- **party\_line\_lead\_initiated\_call\_unsuccessful** — when a lead doesn't confirm they would like to be connected
- **catch\_all\_level1** — when a lead hits CatchAll Level 1
- **catch\_all\_level2** — when a lead hits CatchAll Level 2
- **catch\_all\_level3** — when a lead hits CatchAll Level 3
- **copilot\_paused** — when a lead requires an Mav operator to intervene
- **copilot\_restarted** — when a Mav operator has restarted the conversation

**Outcome** activities are specific to your playbook. To give you an example, a typical Mortgage qualification playbook will include these outcomes that are available for you to subscribe to:

- **callback\_requested** — when the lead has requested a call back from a rep
- **interested — when a lead initially responds to a message**
- **not\_interested — when a lead states that they are not interested (ex: says something like**  
- **party\_line\_completed** — when the lead and the rep have successfully finished a party line
- **qualified** — when the lead has qualified to speak with a rep on a Party Line 
- **unqualified** — when the lead has stated something that disqualifies them from coverage (ex: they reside in an unsupported state) 
- undeliverable — when a message cannot be delivered to the phone number provided
- **opted\_out** — when the lead opts out of messaging, clearly stating a phrase like STOP

Both events and outcomes will post a similar parameters to your supplied URL endpoint and you can expect to see the following parameters for each:

- **activity\_type** — event or outcome
- **activity\_label** — name of event or outcome
- **activity\_play\_id** — Mav ID of the this specific play
- **activity\_note** — summary of activity
- **activity\_created\_at** — timestamp of activity
- **lead\_id** — Mav lead ID
- **lead\_first\_name** — lead first name
- **lead\_last\_name** — lead last name
- **lead\_email** — lead email
- **lead\_opted\_out** — opt out status
- **lead\_created\_at** — timestamp creation date for lead
- **lead\_additional\_info** — array of additional information that is specific to your playbook.
- **lead\_originators**
- **origin** — source name
- **key** — unique ID of originator source

Note: **lead\_orginators** can be the same data you passed on the inbound call. This can be used to match a lead in your system and update the record.

Was this article helpful?

Yes No

### Related articles

- [How do I set a schedule for my Party Line live transfers?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jll2-6qcW7Y8-PT6lZ3nSVPHBPr4rn_w-W6ZFdNP2NsTC2W83vMmm4k10kjW1GW8xj6wWTZtVp_sKl3CvPKrW2SPkfq4KWT1SW3hyN-y90K0z9W7kV1nH8RL91KW1Ml63w6ZGC_6W6g-Gbm3jfQcKVpvR588ZQ7v5W5XBS248XPNhKVrTDfr1C5RQNW52kn1d5YQbTCW1xQ6qH2__SyXW7gjdG_1QTq2pW46m4kZ4D9CJbN86Y4mZKW-0yW91Xw9328wHKLW4_WXZj1WvcqvW37tWKx2FxQ3ZW7C3hH93n54PYVXRzjB573Q8VW3Xd-r93zHmP2W4Rt0VZ2kzf6jW9jhdF_17fvLHf2zYpcP04)
- [How does Mav's Ricochet 360 Integration Work?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/JkM2-6qcW6N1vHY6lZ3pwW9dPXmm6GzWqzW38HDmx85XstLW1Gdw583c2q6YW3V0zZ04Gct5rW28bZWS5Kxpj8W3tZyJP8-PDp7W7kbC9R2W96zqW2tXn1G7dgT6wW6JvL8w455BVTW5Scthr6nsJ_TW5SH-Pm6-_VkKW9gMMsJ2WWWg2W29fYBM7Y-SGCW2KLcy42DK_MKW71Dlh92TNzyhW4l_hxf1TKyFcW4P0rwX8jFGg0W5mvg4c8HGjL5W13T83q8XnD7mW8J4xZr2S76bfW1l7wQq8M9V1NW7TXK8J7BMYNcf53NWX204)
- [Understanding Texting Hours in Mav](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3pjW2QtrHN8sRxrSN4BjTmX-4z2MW3GvBdP55bvSsN2Q45htXqcpRW1DdqQv39mfBXW7BmLNg1dyC6HW4Hskz01BQbDcW5tWQp013vTzHW6y9cW146slxQW1tGGRl8fhG2gW7KrpdJ8Zh5gMW8l1NKZ4QCBlfW2MTh-B4DL0XJW4NjpVC2b7gjMN2W5JJ5YMgw-W1GJ0wr6hltnfN5WzbWDr5gxcW5CY1RL64DG7DW5vJX0x7QcjXgW6wFPFW87p13gW5Pddg21w9Vs6W1N0TM-2YsvnzW7kvJPg7yrHDzW2ZCJNz7T92K5f7VT9Bl04)
- [How do Playbook Alerts work?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3nZW86cxnb3MSwy9W4x_CDY7CZnSCW5PY4r49bwtQfW5sKfzp7MyCMBW67MZXZ1Vlh3PW8xpFyw7JLHxYVFbLHv1d4nBVN27YSF03TBd7W8HZWFs7Pj2Z3W47lzzV4dlzkhW7GFBVJ95vw9lW3LftPl4SJTHZN6lDqcWl8kvqN1SWxfnpJshfW3w3v413TCPbYW7ckLW61byr26N7d4tznQ7Br4N7zXMlv63jc0N6BS50-st4z0N6d2psnm0K-xW3nvch_8hgn79W4zglT26_lXgHW7JBT3j697R2tN6K3_f9pNZK-f30Vxvd04)
- [Party Lines Completed - Feature Reference](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3kXW1jRpXY1SWj7TW9hPcb86FbhDgW4fvLtZ1ySXvJW87XkmW9bjDzpW5fWM-k8Lk5pFW32f58z7zhMpGMLw4DQTsptgN99nPhdxjKJLW4pq1r-6tCLw-W5HzSYV3n5F6MW78ZXjm7nk6_NW2bm7D424yTNhW2WnDcY1Bl1CnW3vVrHL2bb1zRW2--1zJ3Z9qb5W3bLgzn2mqPg-V1g2TL22bgRMVc2zq36zC5M4W68NNtn4zccJlVbbkPL5WBx32VLwFK37-xZ06W7KFBBN3-KMgBW3Vcz8R5BkBrNW2bBj161lq5Nff3HWx0W04)