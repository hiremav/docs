# Source: https://knowledge.hiremav.com/marketing-sources-in-mav

1. [Knowledge Base](https://knowledge.hiremav.com/?hsLang=en)
2. [Integrations](https://knowledge.hiremav.com/integrations?hsLang=en)
3. [Documentation](https://knowledge.hiremav.com/integrations?hsLang=en#documentation)

# Marketing Sources in Mav

### What are Marketing Sources? 

Marketing Sources in Mav lets you create a custom postURL that’s tied to a specific lead source. These URLs act as destinations where lead data can be sent, and each one is automatically tagged in Mav so you can see what’s working and optimize future campaigns.

For example, if you’re sending leads to Mav from two different sources, you can create two different Marketing Sources (one for each) and Mav will tag incoming leads accordingly. No manual tracking needed.

### How it works

1. Go to Integrations > Marketing Sources
 
2. Select “New Marketing Sources”
 
3. Give your source a clear, distinctive name, select the source it’s coming from, and choose the playbook where your leads will be sent
 
4. Click “Save Marketing Source” - Mav will generate a unique **postURL** for you to use.
 
5. Select the link icon to view the Marketing Source Integration Instructions. You can also select the “Email Integration Instructions” to share them with your team.  
 
6. Send leads to that URL via form or JSON
 
7. Mav tracks the source automatically and kicks off the follow-up
 

### How to send leads to Mav

Once you have a postURL, leads can be sent in one of two formats: 

1. Form Submission (URL-encoded) 
 
 1. Send a form submission (like from a website form) using POST to the provided URL. Include fields like: 
 `first_name=Jane&last_name=Doe&phone=1234567890&email=jane@example.com`
2. JSON format 
 
 1. You can also send leads in JSON format: 
 `curl -X POST "https://hiremav.com/marketing_sources/acc_2SbUe8xLqEqrL3/mks_kgaafDRBWshCzp" \` 
   `-H "Content-Type: application/json" \` 
   `-d '{` 
     `"first_name": "John",` 
     `"last_name":  "Doe",` 
     `"email":      "john.doe@example.com",` 
     `"phone":      "5551234567",` 
     `...` 
   `}'`Each postURL can accept either format, and Mav will automatically associate the lead with the correct Marketing Source.
 

### Required fields

To begin sending leads to Mav, the following lead parameters must contain data: 

| 
**Parameter**

 | 

**Description**

 |
| --- | --- |
| 

first\_name

 | 

The lead's given name

 |
| 

last\_name

 | 

The lead's family or surname

 |
| 

email

 | 

The lead's email address

 |
| 

phone

 | 

The lead's phone number

 |
| 

current\_insurance\_carrier

 | 

The insurance company currently providing the policy

 |
| 

current\_insurance\_coverage

 | 

The type or company of the lead’s existing insurance policy

 |
| 

current\_residence\_address

 | 

Full street address of the lead's current residence

 |
| 

current\_residence\_city

 | 

City where the lead currently resides

 |
| 

current\_residence\_state

 | 

State where the lead currently resides

 |
| 

current\_residence\_zip

 | 

ZIP code of the lead's current residence

 |
| 

date\_of\_birth

 | 

The lead's full date of birth (used for quoting and verification)

 |
| 

gender

 | 

The lead’s identified gender

 |
| 

marital\_status

 | 

The lead's marital status (e.g., Single, Married, Divorced)

 |
| 

credit\_rating

 |  Self-reported credit tier (e.g., Excellent, Good, Fair, Poor) |
| 

tcpa\_opt\_in\_token

 | 

TCPA consent token, such as a Jornaya or ActiveProspect unique identifier

 |
| 

tcpa\_opt\_in\_url

 | 

URL to the TCPA proof of consent — often a Jornaya or ActiveProspect screen recording link

 |

 

Was this article helpful?

Yes No

### Related articles

- [Setting up a one-click Slack integration](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3mVW9lTV4b7yYS4YW2XVnn734fnBhW3hjd0d8x5m1lN9cfJCNgq3p1W3X_7B71FvHY7W3MwkSD5fWK0VW2YwfSz8TbwhpW61L_Fc2Vt4YRW7L_Tq97n_TmrN9grnPWB2pLZW6MVzql46bsTQW55N6FX8sjDLFW5VKDgS9dbtykW22nQv33X8f1CW6RFs5c8x0GRrW1Rw8Dt5ldpm9W8JhbY637wCDpW3XKKTQ61v4PKW8bD39L6kyJHbMdmYhShK34lTRVTf1K_ymkW8GXD4W6KXhWCW8yZrtl8cc9nFW8JH-kd6LD8mFf4CHNVY04) 
- [How does Mav's Ricochet 360 Integration Work?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/JkM2-6qcW6N1vHY6lZ3msW4mZtv-7v2TqTN6V6g1GndS8MW6FTKMw4ypDByW2HnZCK91XvvnW5yZGK-7vK12tW4vZ1_T2JZvGgW8HhWj525c2vJW437zWC5PqWgsVNYdZ-42ldK7W4MmVN43gKdmHW8DcWlB4x3-TTW628PwL5WkscxW4_dfdJ7SYJ6mW4KlKSk52MmzXW7CC7FJ7HQZVMW98HsXC40bDY2W1lpxWp37RnNXVCjwNF75K7DzW7DVz_N5lh_8TW78018T38jkNJVdJK3y5bHW03W5HQtv82fhDgZf6JRR-M04)
- [Party Lines Completed - Feature Reference](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3ncW736_H58PdVnmN8x8KKjyc178MGkb1wW13mLW6fmmVk2czkSnW7PX7gv87ZCpqW19W5Qx99vG-QVbSlQC1W6C5YW2yRwTY71lMwpN7Sd_y0BKSk-W2kPF-g1C5QHtW6mw4P_33FMnxW1NnwJ15-9RRfN6VYm55PvWQvW6-zbk41mvrQKN1PNYqPRJ-g6W8FZPg881rH_RW9gDdVd6C7CWBW2F07PL6ft2jDW69hLkv7MJV3SW3-xBlH5PqZ-kW3BzlZG1_N1zsW6l6VQH5l3MKQW8W00gV7PH8CsW3p33S17S5RCff4MR38404)
- [How does Mav's Zapier App Work?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/JkM2-6qcW6N1vHY6lZ3nMW7WllJL911zbBW6p2n_w5v93L9W67KX2B4T9N5YW1h5xVX17HKFQW8yQQSh5SrKfZW1BGcdC3wMyjMW8tRx6M5GljdmN98cffhYp4N_W3PCkm454hX-bW8nDJ-48V23vpW2w1jvg520nKtW6BJsT260chdrW2ZJ6p-4N6BbhW2DC3-X5mg-rsW30BrCx3VxsT3W6DR-5J168Kz4W68DyMS1vMC-8W1gpbfB2y1l6sVRb6FG8N1FZ7VgcmgC1xcjrDVzT_td51CxMgVTl8q16RsnfRf1xr1hP04)
- [Blocked Sources and Scrub Services](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3kKMwy8TmBSMlwVp3MVK7PqqKSW6p6rB_4sr6ChW8vjySX3Gs5zdVgbF_38HckG5W8_1zFm5Q5k7bW121vhM1dq7TyW35X9h66wCmtJW4BxHRJ8MwkyQW1mFZn07fP3pWVXRTJt15ChSyW8Wl62W3HL-kmW28n_sJ6m9WRSW20qgVS2NKqHXW8Xph9h5bXCJmW84Wc0s2YNXgmW1LL3H84ZVx9jW2JFs154qhHnfW7XDXmf2wmbSFVfQDwv6nmFw6W2ltpjf1kxnkmW18x-3Z71Hz84W14HLlV8lPM9BW559jYl3bP4rVf3XMhsH04)