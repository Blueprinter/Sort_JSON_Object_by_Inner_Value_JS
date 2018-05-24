# Sort_JSON_Object_by_Inner_Value_JS
JavaScript - Sort an Object by an Inner Objects Value

Example:

  data = {//This is example data to test the function and show that it works
    'a':{'k1':'P','k2':'blue'},
    'b':{'k1':'Aaa','k2':'red'},
    'c':{'k1':'Z','k2':'green'},
    'd':{'k1':'O','k2':'yellow'},
    'e':{'k1':'BZyetf','k2':'brown'},
    'f':{'k1':'BA','k2':'black'},
    'g':{'k1':'BA','k2':'cyan'}
  }
  
  The above JSON object has an inner object with multiple elements.  The keys to the inner object are named k1 and k2.  In the example code, the entire object is sorted by the inner objects values associated with key k1.
  
  This code does not use a formula in the sort function, because the sort operation is done on a 1D array, which makes the code faster and simplier.  Other strategies to sort JSON data on an inner object's value, first put ALL of the data into an array.  My process does not do that.  My process creates an array, but the array contains only the sort values.  My process does eventually put all of the data into an array, but initially, all the data is transfered to another object, not another array.  Because the data is transfered to another object keyed on the sort values, the data associated with each sort value can be retrieved easily.  The array of sort values is used to retrieve the data back in sorted order by looping through the array of sorted values.
  
  I have not seen any strategy that uses the same process to sort a JSON object by the value of an inner object.
  
