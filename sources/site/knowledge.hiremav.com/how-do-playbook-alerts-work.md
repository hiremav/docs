# Source: https://knowledge.hiremav.com/how-do-playbook-alerts-work

1. [Knowledge Base](https://knowledge.hiremav.com/?hsLang=en)
2. [Analytics, Reporting & Alerts](https://knowledge.hiremav.com/analytics-reporting-alerts?hsLang=en)

# How do Playbook Alerts work?

## Playbook alerts allows you to programmatically respond to changes in positive intent or outcome rates by source or date.

To access Playbook Alerts, browser over to "Playbooks" and then click the "Alerts" button on the playbook you would like to set an alert for.

![](https://knowledge.hiremav.com/hubfs/Screenshot%202023-06-08%20at%208-41-43%20AM-png.png)

Once inside, you can create a new alert by clicking on the "New Alert" button.

![](https://knowledge.hiremav.com/hubfs/Screenshot%202023-06-08%20at%208-43-24%20AM-png.png)

An alert has the following configurable options:

- **When** _(Monitor Type)_ \- This is either [**Positive Intent Rate** or **Outcome Rate**](https://knowledge.hiremav.com/what-are-mavs-reporting-events?hsLang=en)
- **On** _(Alert Type) -_  This is either **Date** or **Source**
- **Comparison** \- **Is Greater Than** or **Is Less Than**
- **Metric Alert Threshold** - Numeric percentage metric for the alert threshold
- **Webhook URL** - The publicly accessible webhook URL to receive the JSON payload with alert details.

**Webhook Payload Information** - If an alert is active and gets triggered Mav will send a JSON payload with details on the alert, metric and playbook. Here is an example of that payload:

{ 
 
alert: { 
 
monitor\_type: PositiveIntentRate 
 
alert\_type:Date, 
 
alert\_metric: 5, 
 
apert\_metric\_comparison: islessthan, 
 
note:  OutreachPlaybookAlert-PositiveIntentRateonDateislessthan5%, 
 
datetime: 2023-06-02T10:41:13.704-07:00 
 
}, 
 
metric: { 
 
metric\_type: Date, 
 
date: 2023-06-02, 
 
source: source\_a, 
 
sub\_source: subsource\_b, 
 
leads: 1, 
 
wins: 0, 
 
win\_percentage: 0 
 
postive\_intents:0, 
 
positive\_intent\_percentage: 0, 
 
win\_to\_positive\_intent\_percentage: 0 
 
}, 
 
playbook: { 
 
id: pbk\_wtBPCUDFJDppvD, 
 
name: Outreach 
 
} 
 
}

Was this article helpful?

Yes No

### Related articles

- [How do I set a schedule for my Party Line live transfers?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jll2-6qcW7Y8-PT6lZ3p-W8nMmb539hS-VW2zvjgV1tgQrHW21njFj5t_MY4W4q0SF55JrZ3fVqQNVx63c2vBW60PTjY1-DYVWN92XnN-cTYJ8N7FCjgscB_R7W3-wZn_76GqkKW77s_Mf7Pvww7V8mTvR5zQqT3W4K5wzK7vKyXFW12g75m3bYrQDW3hpYYt5pSsymMMzMkcPGtDLW7dqWlG3tKFf5W8Kkzvv5ZxdWyW7K01Hz1DZGD8W2yDh196d_7f-N12mxRKWf0kNW14kHmF8_s6HwW89w3VT8lDrrCW7rTS5R20XQ1BN1lsLt7wCXLQW6WPPRT4zdkrTW7mwR-06kZPGkf96xk4H04)
- [How does Mav's Ricochet 360 Integration Work?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/JkM2-6qcW6N1vHY6lZ3njN7V4TvYy-PPCW6H7HN53sLBsQN82KKKx_PTSxW4JGJNg6khBS9W4QQzxX7ff6KdW6k-b_f820ry3W3ZwhkM4wLf_mW5ZpbTH8xNCgQVDqrVW6T6Kf5N6kNP7Sl7vHKN2TyKN5XJ-kJW3k2zs81VSDF4W2l7MDL87Y0HBW3GvK6Q3Czxp-W1yjpZL70X0K-W5yc2Sh2wPGhgV-03-y70B-HsW5Jq78k6m-g5-W3djx9x4QjCk8W4gyrbb5kbYNQW3Pb_2k4mSs4TW6hxcb6478Z01f7Wn1mv04)
- [Party Lines Completed - Feature Reference](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3lCW3klhzS7yW_MQW7LnWyR39vd70W6cvn3L6cf44_W5WV7nz2d0RlKW6lHlMG5vfMj5W8n83Yr3YZt2pW7ZkDkF4229fPN8XB4mLy4vf9W2wrLY33GltF1W4K1Q-Y1v8v4TW5MslKD7clcWRW8rLvGR42n38CW7GT8tq2VvyWjW6l-8v-70V7-0W7gdSQd6Nh99rW7dD02m6zgN5hW2XcdMd2nWnzQW1bNbjC431YJ7Mxn-PFV9skDW7cLVQJ3VKdfkW27gDbw41J529W1XmGpl7yYTFFW5JL3gD3dmnpCW8h751L66n1T7dDBM6H04)
- [How does Mav's Zapier App Work?](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/JkM2-6qcW6N1vHY6lZ3pjW7vQmb94Hf0q_VckKSK5DcNPPW8qnLdr2F3dj2W2NxgPB54sx5wW4TzW7w5pB28jW6CzCrm9jV8pzN1XGdPFxshp9W99tkwt4n13G0W1FGxPZ6Szj8NW6_yRjt89q803V_dSFk6QTtYJW3GHQ-L5mqTdDW3wmCD35fX_77W655VPG1mFMQyW2FLK_H4ZmrwsW7HvfW81wq0K4VpVkpJ6gGgkFN3GPBfd5TMVQW3-yRsb8Lr1DpW71fzgz4nmQWrW45sGYM5v5rmKW2JFR3g21wZ4lf2fQRsM04)
- [Understanding Texting Hours in Mav](https://knowledge.hiremav.com/e3t/Ctc/W1+50013/cMVLj04/Jl22-6qcW7lCdLW6lZ3kSW1FrkZ236C2h6Vl667N6qMqbvVG_hVP8RBnTkW7MR8mr4kB01vW51SBCL7cxCZ3W5TlmHg6xV3kcW4bcDmy7hwV0pW2X4qS93T8v3RW8NKn442F1yQ4W7lzQX87Flk6sW4XZK785w83j8VRjTm92NSRP2W8XjgmD96F_NKM5x3wwpYYs2W2dMlSY7WQr1pW6fNLZR461CSDW5VGTw86CwNtvW5Xx0HK5hB6T9W2p-6jx6-kKD9N42PHVf6FrzLW2n-v1450Sv2vW74Sz_p2n2ZMFW4Yxr674KthN2W2NCKRD499z9ddrRGf604)