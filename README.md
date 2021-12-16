# README
This purpose of this was automate the process of checking how much a rental property's price had declined since its peak price prior to pandemic lockdowns.

## Files and Folders
- `crawler.ipynb` does all the work
- `input\targets.txt` should contain a line for each of the properties you are interested in checking. Data is the format:
  
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

