 
# chi2021data

We anonymously provide this dataset for the rebuttal to our CHI2021 submission (#2585). Upon acceptance, we will add more documentation for the variables and details on how the data were collected. We will also likely move this repository to one of the authors' GitHub accounts.

**Rows**

Each row corresponds to a single email-reply scenario judgement.

**Columns**

```
# Judgement IDs
JudgeID : An anonymous judge ID
pair_id :  a unique ID for the email-reply pair
scenario_id : a unique ID for the scenario (email-reply + social tie + structure)

# Judgement metadata
category : the category for the email-reply pair
social_tie : the social tie the email is from
email_structure : a boolean for whether the greeting/closing were included
counterbalance : the counterbalancing group
hierarchy : factor indicating whether relationship has low or high hierarchy
relationship : factor indicating relationship type (professional, personal, family)
timer : time in seconds spent on this judgement
timer_bins_meta : binned time variable

# Judgement content 
email_from : who the email is from
email_greeting : the greeting used at the top of the email
email_closing : the closing used at the end of the email
email_body : the body of the email being judged
email_context : the first sentence of the email
email_act : the second sentence of the email
email_reply : the reply to the email

# Likert ratings
appropriate : Likert scale rating for how the appropriate the reply is
positive : Likert scale rating for how the positive the reply is
polite : Likert scale rating for how the polite the reply is
professional : Likert scale rating for how the professional the reply is
sufficient : Likert scale rating for how the sufficient the reply is

# Binary and free text responses
would_send : a binary response indicating if judge would send email as is
adjustment : text response, how the judge would adjust to the email before sending it
adjustment_rationale : text response, the judge's rationale for their adjustment
adjusted : a boolean indicating if the judge changed the reply

# Word counts and classifications
num_words_{email_body,email_reply,adjustment} : number of words in each text column
num_char_{email_body,email_reply,adjustment} : number of chars in each text column
short_email : boolean classification of email
num_words_diff_adjustment : number of words added or removed while adjusting the reply
```
