# Data Dictionary

## campaigns.csv
Campaign-level metadata used to evaluate marketing efficiency.

**Example fields**
- `campaign_id`: unique campaign identifier
- `campaign_name`: campaign name
- `channel`: marketing channel
- `spend`: campaign spend
- `start_date`: campaign start date
- `end_date`: campaign end date

## dealers.csv
Dealer reference table used for dealer-level performance comparison.

**Example fields**
- `dealer_id`: unique dealer identifier
- `dealer_name`: dealer name
- `region`: dealer region
- `province`: dealer province or area

## leads.csv
Lead-level table containing lead creation and assignment information.

**Example fields**
- `lead_id`: unique lead identifier
- `dealer_id`: assigned dealer
- `campaign_id`: source campaign
- `model_id`: vehicle model
- `lead_created_date`: lead creation timestamp
- `lead_source`: lead source channel

## interactions.csv
Interaction history used to measure response time and follow-up behavior.

**Example fields**
- `interaction_id`: unique interaction identifier
- `lead_id`: linked lead
- `first_response_time`: first response timestamp
- `follow_up_within_24h`: whether follow-up happened within 24 hours
- `response_minutes`: response time in minutes

## outcomes.csv
Lead outcome table used to evaluate qualification and sales conversion.

**Example fields**
- `lead_id`: linked lead
- `is_qualified`: whether the lead became qualified
- `is_won`: whether the lead converted to a won deal
- `outcome_date`: final outcome date

## models.csv
Vehicle model reference table used for model-level comparison.

**Example fields**
- `model_id`: unique model identifier
- `model_name`: vehicle model name
- `segment`: model segment
