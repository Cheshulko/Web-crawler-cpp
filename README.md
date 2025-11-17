# Just another one Web Crawler

## Overview
The crawler starts from a specified URL. It requests that URL and searches the page for an input pattern.

The result is either a success or a failure. For successful results, it counts occurrences of the pattern on the page.

It extracts all hyperlinks from the retrieved pages and adds them to the list of URLs to visit.

## Input
Initial URL, number of threads, number of URLs to scan, and pattern to search for

## Output
List of scanned URLs marked as Succeeded/Failed, occurrence counts for the pattern, and URLs found on each page to visit

## Environment
* Qt 5.15.2
* cmake 3.5
* C++17

## Build
```
  1) mkdir build 
  2) cd build/
  3) cmake .. -DCMAKE_PREFIX_PATH=<path_to_qt_lib> 
  <br>(cmake .. -DCMAKE_PREFIX_PATH=/Users/mykyta/Qt/5.14.2/clang_64/)
  4) make -j6
  5) ./x64/bin/MultiWebSearcher
  <br>??? 
  <br>PROFIT
```
  
## UI

![](Screenshots/Screenshot1.png)

## License
MIT  
