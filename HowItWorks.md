#Library Initialization
1. All elements which have render-if loop over them one by one
2. Get the attribute and evaluate each expression (this will populate the the selector array)
3. Loop over the selector array and attach "change click" handler to the selectors in the array
   (Use delegated events using on)
   https://learn.jquery.com/events/event-delegation/
   delegated parent : "body:first" #TODO make this dynamic in future.
4. Trigger change event for all the elements in the array
