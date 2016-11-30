## Sets [Back](./../data_structure.md)

A set is a collection of unique elements, in which elements are also called **members**. 

### Sets Definition

A set containing no members is called the **empty** set. The **universe** is the set of all possible members.

If two sets contain exactly the same members, we consider them as equal.

A set is consider a **subset** of another set if all the members of the preceding set are contained in the following one.

```js
function Set() {
    this.dataStore = [];
    
    /** methods */
    this.add = add;
    this.remove = remove;
    this.show = show;
    
    /** set operations */
    this.size = size;
    this.union = union;
    this.interset = interset;
    this.subset = subset;
    this.difference = difference;
}

function add(data) {
    if (this.dataStore.indexOf(data) < 0) {
        this.dataStore.add(data);
        return true;
    } else {
        return false;
    }
}

function remove(data) {
    var index = this.dataStore.indexOf(data);
    
    if (index > 0) {
        this.dataStore.slice(index, 1);
        return true;
    } else {
        return false;
    }
}

function show() {
    return this.dataStore;
}
```

### Set Operations

```js
function contain(data) {
    if (this.data.indexOf(data) < 0) {
        return false;
    } else {
        return true;
    }
}

function union(set) {
    var tmpSet = new Set();
    var storeLen = this.dataStore.length;
    
    for (var i = 0; i < this.dataStore.length; i++) {
        tmpSet.add(this.dataStore[i]);
    }
    
    for (var i = 0; i < 
}
```