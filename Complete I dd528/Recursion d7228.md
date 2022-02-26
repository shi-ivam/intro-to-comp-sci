# Recursion

A Function that calls itself

```jsx
function countTo(max,current,list){
	if (current > max) return ;
	console.log(max);
	countTo(max,current+1);
}

const counts = countTo(5,1,[]);
```

### When is recursion useful?

It is useful when you can divide you problem into smaller pieces of the same problem

Example : The Fib Sequence

```jsx
function fib(n){
	if (n == 2 || n == 1){
		return 1;	
	}else if (n <= 0){
		return 0;	
	}
	return fib(n-1) + fib(n-2)
}
```