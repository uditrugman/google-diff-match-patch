# google-diff-match-patch

The Diff Match and Patch libraries offer robust algorithms to perform the 
operations required for synchronizing plain text.

1. Diff
	* Compare two blocks of plain text and efficiently return a list of differences.
1. Match
	* Given a search string, find its best fuzzy match in a block of plain text. 
  Weighted for both accuracy and location. 
1. Patch
	* Apply a list of patches onto plain text. Use best-effort to apply patch 
  even when the underlying text doesn't match.  
  
Currently available in Java, JavaScript, Dart, C++, C#, Objective C, Lua and 
Python. Regardless of language, each library features [the same API](https://code.google.com/p/google-diff-match-patch/wiki/API) 
and the same functionality. All versions also have comprehensive test harnesses.  
  
### Algorithms

This library implements [Myer's diff algorithm](http://neil.fraser.name/software/diff_match_patch/myers.pdf) 
which is generally considered to be the best general-purpose diff. A layer of 
[pre-diff speedups and post-diff cleanups](http://neil.fraser.name/writing/diff/) 
surround the diff algorithm, improving both performance and output quality.

This library also implements a [Bitap matching algorithm](http://neil.fraser.name/software/diff_match_patch/bitap.ps) 
at the heart of a flexible [matching and patching strategy](http://neil.fraser.name/writing/patch/).

### Dart code

The dart version of the code is being hosted at https://github.com/financeCoding/google-diff-match-patch 
for the time being. 