# ova-finder-prototype

This prototype can be edited and used for user research sessions or just having a visual representation of what your finder would look like in the end. 

Fork or take a copy of this repository and create your own version of a finder

## Places to edit
`home.html` for main copy of the finder 
`filters.html` for the list of filters you want 
`subpage.html` to change what the subpages will look like 
`filters.js` to change the filtering functionality 

## Gotchas
make sure the "value" of your filters match exactly what is in the organisation data 
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
The value in mental health corresponds exactly to `helpsWith: ["mental health"],`

## Disclaimer
There are probably bugs in this, but as it is for prototyping purposes it should be fine. 
