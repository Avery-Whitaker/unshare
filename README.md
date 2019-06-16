# unshare

Python extension for C's unshare call. <br>
See [man 2 unshare](http://man7.org/linux/man-pages/man2/unshare.2.html).


## Usage

`unshare(flags)`

Supported flags: `CLONE_NEWNS`, `CLONE_NEWUTS`, `CLONE_NEWPID`, `CLONE_NEWUSER`, `CLONE_NEWIPC`, `CLONE_NEWNET`, `CLONE_THREAD`.

Multiple flags can be used using the bitwise or operator.

## Example usage

```python3
import unshare
unshare.unshare(unshare.CLONE_NEWUTS)
```

The following screenshot is taken from a sample script which uses the unshare library.

![](https://i.imgur.com/B8X0LT8.png)