# Hello 👋

My name is Mrinmoy Dutta and I'm a 2nd year computer science student at UCSD. Here I'll share some projects that I've been working on.

Some of the programming languages that I've worked in are as follows:

- Java
- C++
- Python
- Dart
- Bash

## Projects

### Weather App

I created this site to learn how to make a website as well as get information through API calls. [**Github :octocat:**](https://github.com/lukedutta9/weather-app)

![](assets/weather-app.png)

### Other Project Ideas

Some other project ideas that I have are:

 - [ ] ML model that learns how difficulty ratings work in osu!
 - [ ] Web Chat Room

## Other Random Stuff

### Functional Programming
In my CSE 130 class (Programming Languages) I learned about functional programming, specifically with the language Haskell. It just absolutely ***blows my mind*** with how it works.

Here's an example of quicksort in a "typical" language

```java
void sort(int arr[], int beg, int end){
  if (end > beg + 1){
    int piv = arr[beg];
    int l = beg + 1;
    int r = end;
    while (l != r-1)
       if(arr[l] <= piv) l++;
       else swap(&arr[l], &arr[r--]);
    if(arr[l]<=piv && arr[r]<=piv)
       l=r+1;
    else if(arr[l]<=piv && arr[r]>piv)
       {l++; r--;}
    else if (arr[l]>piv && arr[r]<=piv)
       swap(&arr[l++], &arr[r--]);
    else r=l-1;
    swap(&arr[r--], &arr[beg]);
    sort(arr, beg, r);
    sort(arr, l, end);
  }
}
```

Now in a functional language
```haskell
sort []     = []
sort (x:xs) = sort ls ++ [x] ++ sort rs
  where
    ls      = [ l | l <- xs, l <= x ]
    rs      = [ r | r <- xs, x <  r ]
```

While these implementations don't line up completely, it's still really cool how we're able to write algorithms in other ways through functional programming. It helps give a different perspective on programming as a whole.

### My Senior Quote
> "Sounds like a you problem"