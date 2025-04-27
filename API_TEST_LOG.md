# PRAISE CAGE API TEST LOG

## OVERVIEW
- Tester: Tim Baines
- Testing Date: April 27, 2025
- Respository: https://github.com/pchinjr/praise-cage-rest-api-workshop 
- Environment: Github Codespaces
- Testing Tools: val town

### **Getting Started with HTML and an HTTP Endpoint**

1. GET praises
 - Status: ✅ PASSED
 - Description: After submitting a form entry, the page will display JSON output with all recorded praises. Open the endpoint URL in a browser (GET request) to view stored praises in JSON format.
 - Request: GET https://timbaines-responsibleyellowaphid.web.val.run/

 ```
 json output
 {
    "success":true,"praises":
    [
        "test","ttest3","ttest3","04/27/25 Praise Cage Test"
        ]
}
 ```

 - Expected Response: JSON array of praises objects with status of 200

```
json format (get request)
[
    "test",
    "ttest3",
    "ttest3",
    "04/27/25 Praise Cage Test"
]
```

- Response Time: 510ms