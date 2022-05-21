# This is Kun Wang CSE15L lab report 3

Kun Wang

Professor Soosai Raj

21 May 2022

## MarkdownParse Snippet tests:

Repositories used:
- [My Repo](https://github.com/KunWang0129/markdown-parser)
- [Reviewed Repo](https://github.com/yuxinguo13/markdown-parser.git)

Tests in `MarkdownParseTest.java`:
- Variables used:
![Variables](/lab4content/SnippetLinks.png)
- Test for my `MarkdownParse.java`:
![MyTest1](/lab4content/MDPTestPt1.png)
![MyTest2](/lab4content/MDPTestPt2.png)
- Test for reviewed `MarkdownParse.java`:
![ReviewTest1](/lab4content/ReviewTestPt1.png)
![ReviewTest2](/lab4content/ReviewTestPt2.png)

Results for my implementation:
- In short, non of the three tests passed, here are the specifics:
![MyResult](/lab4content/MyTestResult.png)
- All of the errors are assertion errors, which means my implementation was not able to capture the correct link for each test.

Result of reviewed implementation:
- In short, non of the three tests passed, here are the specifics:
![ReviewResult](/lab4content/ReviewTestResult.png)
- There is a memory and an out of bound exception, which the implementation needs further fixes.

## Solution to the tests

Fixes for snippet 1:
- There should be a small fix for the inline code with backticks senario, as the major factor is the indices of these backticks. Nothing major should be changes to the original code.
- The major factor to fix is make sure there isn't an odd number of backticks within the brackets, which will omit the link.
- Here's a demo of what the fix might look like.
![snippet1fix](/lab4content/Snippet1Fix.png)
- Note that the fix might not be completed as it is only used as a demonstration of why major code changes may be unnecessary.

Fixes for snippet 2:
- There would be a major fix on the original code for the cases in snippet 2. Because we would have to completely overhaul the preexisting mechanism of how to detect links in our `MarkdownParse.java`.
- Specifically, the ways to detect open and close parenthesis and brackets need to be revised, therefore this requireds a more involved change.

Fixes for snippet 3:
- There should be a small fix on the original code for cases in snippet 3. 
- The major concerns for these test cases are the blank spaces and newlines. A few lines of simple restrictions should be able to fix the issue.

