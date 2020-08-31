Doc string:

```
  """
    Return a 2-D array with ones on the diagonal and zeros elsewhere.
    
    Parameters
    ----------
    N : int
      Number of rows in the output.
    M : int, optional
      Number of columns in the output. If None, defaults to `N`.
    k : int, optional
      Index of the diagonal: 0 (the default) refers to the main diagonal,
      a positive value refers to an upper diagonal, and a negative value
      to a lower diagonal.
    dtype : data-type, optional
      Data-type of the returned array.
    order : {'C', 'F'}, optional
        Whether the output should be stored in row-major (C-style) or
        column-major (Fortran-style) order in memory.
        .. versionadded:: 1.14.0
    
    Returns
    -------
    I : ndarray of shape (N,M)
      An array where all elements are equal to zero, except for the `k`-th
      diagonal, whose values are equal to one.
    
    See Also
    --------
    identity : (almost) equivalent function
    diag : diagonal 2-D array from a 1-D array specified by the user.
    
    Examples
    --------
    >>> np.eye(2, dtype=int)
    array([[1, 0],
           [0, 1]])
    >>> np.eye(3, k=1)
    array([[ 0.,  1.,  0.],
           [ 0.,  0.,  1.],
           [ 0.,  0.,  0.]])
    \"\"\"
    ```
From https://github.com/numpy/numpy/blob/v1.14.2/numpy/lib/twodim_base.py#L140-L194


Function equivalent to round():
```
# Put your test code here

num = 3007123.14152936
places = -2
print("round: ", round(num, places))
#print("round with negative places: ", round(num, -places))


print( "floor division: ", ( num // (10**(-places)) )*(10**(-places)) )

def round2(numb, places):
    return ( numb // (10**(-places)) )*(10**(-places))

print("round2: ", round2(num, places))
```
