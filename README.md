# README
This project is about easily finding out how much a rental property's price had declined since its peak price prior to pandemic lockdowns.

## Get Started
To run this project, open `crawler.ipynb` as a Jupyter Notebook, and run reach cell.

### Parameters
A cell near the top of `crawler.ipynb` contains the following parameters:
- `__from_cache_file` - if `True`, the crawler will take `html` from the specified cache file rather than request html from the internet. 
- `__targets` - the source of target addresses
- `__cache_dir` - the location of cached html
- `__data_output_file` - name of the output file
- `__output_dir` = directory for any and all output that is written to file

## Files and Folders
- `crawler.ipynb` does all the work
- the file specified by `__targets` should contain a line for each of the properties you are interested in checking. Data is the format:
  
```
    <unit #>/<street number> <street name>, 
    <suburb>, 
    <state(2-3 letter abbreviation)> <postcode>; 
    <advertised price($)>; 
    <number of bedrooms>; 
    <is this an NRAS property? (y/n)>
```
  - 
    - **Note:** Each entry should be on a single line. The above is broken over several lines for readability
    - **Example:** <br> 301/4 Pretend Place, Newtown, NSW 2067; 290; 1; y

