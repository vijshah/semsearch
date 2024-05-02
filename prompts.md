# QUE: Query Understanding and Expansion

- Simple Prompt
<pre>
Task: Expand this search engine query "find nvidia comparables".

Be concise, do not provide explanations. Final JSON should look like below.

[json]
{
"companies": [list of companies explicitly mentioned in the query],
"places": [list of countries and regions explicitly mentioned in the query],
"industry": name of one industry that is most relevant to the query as per GICS classification,
"sector": name of one sector that is most relevant to the query as per GICS classification,
"alternatives": [list of 10 keyword search terms]
}
[/json]

Response:
</pre>

- Sample Output
<code>
{
  "companies": ["Nvidia"],
  "places": [],
  "industry": "Semiconductors",
  "sector": "Information Technology",
  "alternatives": ["Nvidia comparable companies", "Nvidia peers", "Nvidia competitors", "Nvidia similar companies", "Companies similar to Nvidia", "Nvidia peer comparison", "Nvidia competitors in semiconductors", "Nvidia comparable firms", "Nvidia industry peers", "Nvidia competitors in technology"],  
}
</code>

