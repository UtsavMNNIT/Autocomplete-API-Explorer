1-> API-testing
This repository includes a Python script to detect and remove names from an automatic full API hosted on 'http: /35.200.185.69: 8000'. 
The project tests various API versions ('v1', 'v2', 'v3') and counts the number of requests made to get all names.

2-> Project Overview
The project aims to interact with '/VX/Autocomplete' closing points (where `X` version is:' v1 ',' v2 ',' v3) An API, remove all possible names, and count the number of requests made. 
The API uses prefix-based autocamplit (eg, `Query = ab` Return Name 'ab')
and has a rate of 100 requests per minute.

3-> key features
 Script `v1 ',' v2 ', and' v3 'for API versions.
 Esinkronous request using 'AIOHTP' for rapid execution (alternative sequential version using requests).
 If obstructed, cashing to resume extraction.
 Request counting to track the total number of API calls.
 Logging for debugging and progress tracking.

4-> API findings
 Closing point **: `/vx/Autocomplete? Query = <prefix> `
 Rate Limit **: 100 requests per minute (confirmed for 'V1' and 'V2', taken for 'V3').
 Result limits **: 10 names per request (for V1 'and V2', should be confirmed for 'V3').
 Pageination **: Not supported (for V1 'and V2', should be confirmed for 'V3').
 sorting **: not supported (tested with 'sort = desc` on' V1 ').

5-> files
 Extract_names_v1.py`: Script '/V1/Autocomplete` (Esinkronus).
 Extract_names_v2.py ': Script'/V2/Autocomplete` (asynchronous).
 `Extract_names_v3.py ': Script'/V3/Autocomplete` (asynchronous).
 `Extract_names_v3_chipational.py ':'/V3/Autocomplete 'using sequential version requests.
 'names_v1.txt `,` names_v2.txt`, `names_v3.txt`: output files which have extracted names.

6-> requirements
- Pythan 3.x
- to install
