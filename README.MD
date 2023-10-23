
# 🦀->🐍 result: Rust feature comes to python.

## FAQ:

[There already exists a package, that does exactly that](https://pypi.org/project/result/), but i want to add a few custom modifications,that i miss, and they doesn't exists in Rust (as i know atm), a new features, that may not be for everyone.

### These features are:

- 📑`Success`, `Failure` Types:
	Instead of returning just a status of function/method completion,
	if it executed with or without errors, we can also let user know, if it also did what user was asking, or not.

	Success and Failure will be both of `Ok` type, while `Err` will be on its own.
	
	**Why?**
	To replace a standard way of handling it via `True` and `False`.

	1. you would be able to return/recieve `Success` or `Failure`.
	1. for cases where you want to return data and status:
		Instead of doing:
		```py

		return {success:  True, data:  ...}

		```
		you would be able todo
		```py

		return Success(data)

		```

	consistency and ease of use.

- ✍️`log` method:
	a method to add message (and if nessesary, a description) containing an information, that will be useful for logging porpouses.

	devs can provide a message, that can be logged by users, that are using loggers.

  

## 👀 Detailed description:

*description will come soon...*