# Atlassian-Custom-Reporting-
Endpoints url, which one to use?
https://atlassian-report-59747f021db0.herokuapp.com/atlassian/report/${eventId}/${registrantId}
These are merge fields that we can put from swoogo, url parameters. 

Check in the widget or js snippet down where it checkbox is selected. 
Example 
 <div id="registrantId">*/registrant-id/*</div>
    <div id="eventId">*/event-id/*</div>

    Where is the info coming from? 
    The attendee information shown (number attended, etc.) is populated dynamically by Swoogo from registrant activity stored in their backend database, associated with IDs in HTML like <div id="registrantId">. The animateNumber function reads these numbers from the page to display them, but the actual values are injected by Swoogo after the user logs in and interacts with the event.

What happens when you click it? 
Nothing it is just a static widget? 

How do you test it? 
-Use a test or dummy registrant/account, participate in sessions or sponsor kiosks, then refresh the dashboard to see if numbers update.
-Change the number in the HTML or JavaScript for local testing, but this won’t reflect actual backend data—real data only updates via Swoogo’s API/events.
    Where did the attended number come? Ask Tate
    How many hours are remaining in the custom reporting? Ask Tate
