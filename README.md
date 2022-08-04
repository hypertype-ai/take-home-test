# Hypertype Take Home Assignment

Programming language: `Javascript`, `Python`, `Go`

Use any librairies you like.

⚠️ Document how to run the code and the tests.


## Instructions

Retrieve the data from the endpoint.
It returns a time series containing the number of emails per day

Tasks:
- calculate the total number of emails
- caclulate the average number of emails
    - per week
    - per month
    - per year
- calculate the median number of emails
    - per week
    - per month
    - per year
- write unit tests


### example of request

```js
fetch(`${ENDPOINT_URI}/${PATH_URI}`, {
  headers: {
    Authorization: `Bearer ${token}`
  }
})
.then((res) => res.json())
```

### example of response

```js
response = {
  id: "144ef415-92a4-46fe-91ec-5e442cd69540",
  name: "User 133",
  total_emails: 960,
  series: [
    {ts: 1629634975, v: 9} // ts = timestamp
    {ts: 1629721375, v: 52} // v = the number of emails received
    ...
  ]
}
```
