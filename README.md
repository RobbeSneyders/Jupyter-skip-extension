# Jupyter-skip-extension

This is a Jupyter kernel extension that adds the ability to skip the execution of a cell via the skip magic command.

Load the extension in your notebook:

```Jupyter Notebook
%load_ext skip_kernel_extension
```

Run the skip magic command in the cells you want to skip:

```Jupyter Notebook
%%skip True
```

You can use a variable to decide if a cell should be skipped by using $:

```Jupyter Notebook
should_skip = True
%%skip $should_skip 
#skipped

should_skip = False
%%skip $should_skip 
#not skipped
```
    
