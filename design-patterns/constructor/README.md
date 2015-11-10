
### Constructor Pattern
Object constructors are used to create specific types of objects - both preparing the object for use and accepting arguments which a constructor can use to set the values of member properties and methods when the object is first created.

```javascript

    (function () {

	    function Car(model, year, miles) {
	        this.model = model
	        this.year = year
	        this.miles = miles
	        this.toString  = function () {
	            return this.model + " has done " + this.miles + " miles";
	        }
	    }

	    // We can create new instances of the car
	    var civic = new Car("Honda Civic", 2009, 20000);
	    var mondeo = new Car("Ford Mondeo", 2010, 5000);

	    // and then open our browser console to view the
	    // output of the toString() method being called on
	    // these objects
	    console.log(civic.toString());
	    console.log(mondeo.toString());

    })()

```

*For complete reference, click [here]*(http://addyosmani.com/resources/essentialjsdesignpatterns/book/#constructorpatternjavascript).