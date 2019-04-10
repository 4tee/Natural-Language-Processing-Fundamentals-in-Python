# Which pattern? #

Which of the following Regex patterns results in the following text?

```python
my_string = "Let's write RegEx!"
re.findall(PATTERN, my_string)
['Let', 's', 'write', 'RegEx']
```

In the IPython Shell, try replacing PATTERN with one of the below options and observe the resulting output. The `re` module has been pre-imported for you and `my_string` is available in your namespace.

## Answer: PATTERN = r"\w+" ##