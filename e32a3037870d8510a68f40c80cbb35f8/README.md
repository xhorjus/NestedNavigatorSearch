# Nested Navigator Search (ServiceNow)

This ServiceNow application adds the possibility of a performing nested search using the application navigator's filter. A nested search is a search for a certain menu entry with a filter set on the module/app's name.

# Use case

For instance, the user searches for `Properties`. Considering there are quite some modules that have a `Properties` menu, this can easily return tens of results. If I am only interested in the properties for `Field Service`, I will have to use the browser's page search to look for the respective item on the page - but this is sub-optimal.

# How to use 

Using this extension, the user first typs `field se,` (partial, case-insensitive search is supported), where typing the comma at the end now sets a parent module filter on `field se`. This is reflected in the placeholder of the filter. Afterwards, searching for `prop` returns `Properties`.

An active parent filter can be cleared by either clicking the `X` to clear the current search (thus clearing the parent filter) when an input is present, or by typing only a comma with no parent value `,` in the bar. 

# How to install

1. Ensure you have an account on GitHub with (ssh) access keys added, so you can import the repository into Studio. 
2. Fork this repository so you have a copy on your own Github account. Unfortunately, this is required by Studio at this time.
3. Open Studio and import your forked repo from source control.

A new global application `Nested Navigator Search` should now exist within the system, injecting the search logic into the navigation filter.
