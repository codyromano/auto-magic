# auto-magic
Automatically convert a large HTML &lt;select> box into an &lt;input> field with autocomplete

## Configuration

| Option                             	| Type     	| Description                                                                                                                               	| Required 	|
|------------------------------------	|----------	|-------------------------------------------------------------------------------------------------------------------------------------------	|----------	|
| selectNode                         	| DOM Node 	| The select box to be replaced                                                                                                             	| Yes      	|
| maxResults                         	| Integer  	| How many autocomplete results to display at once                                                                                          	| Yes      	|
| initialRender                      	| Function 	| Must return a DOM node for the autocomplete form that will replace the <select> box.                                                      	| No       	|
| render(state)                      	| Function 	| Handles DOM mutations after the initial render. It receives a plain object representing state (e.g. if there is input in the search box). 	| No       	|
| onSuggestionClick(suggestionValue) 	| Function 	| Fires after an autocomplete suggestion is clicked                                                                                         	| No       	|
| onSuggestionHide                   	| Function 	| Executes after the suggestions list is hidden                                                                                             	| No       	|
| onSearchTermEntered(searchTerm)    	| Function 	| Called after the user enters input   
