# ova-finder-prototype

This prototype can be edited and used for user research sessions or just having a visual representation of what your finder would look like in the end. 

Fork or take a copy of this repository and create your own version of a finder

As this is created using the Gov.uk prototype kit, it is easily hostable on Heroku as per the prototype instructions: https://prototype-kit.service.gov.uk/docs/publishing

## Running this code 
As this code is using the prototype kit, it is simple to run this project with the following command

`npm run dev` 

Navigate to `http://localhost:3000/finder/home` 

## Places to edit
`home.html` for main copy of the finder 

`filters.html` for the list of filters you want 

`subpage.html` to change what the subpages will look like 

`filters.js` to change the filtering functionality 

## Gotchas
Make sure the "value" of your filters match exactly what is in the organisation data 
For example: 
``` 
{{ govukCheckboxes({
                  name: "health",
                  classes: "govuk-checkboxes--small",
                  items: [
                    {
                      value: "mental health",
                      text: "Mental health"
                    },
                    {
                      value: "physical health",
                      text: "Physical health"
                    },
                    {
                      value: "social care",
                      text: "Social care"
                    }
                  ]
                }) }}
```
The value in mental health corresponds exactly to the organisation data `helpsWith: ["mental health"],`

## Disclaimer
There are probably bugs in this, but as it is for prototyping purposes it should be fine. 
