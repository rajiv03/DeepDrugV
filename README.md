## DeepDrugV
DeepDrugV constructs the voronoi diagram (VD) of protein binding site/pocket or ligand structure based on the 3D  or 2D coordinate structure.

## Requirements
1. Python 2.7+
2. numpy 1.14+
3. scipy 0.18+
4. Pandas 0.19+
5. scikit-spatial 0.12.0
6. matplotlib 2.0.2+
7. biopandas ; eg : pip/conda install biopandas  

## Getting started

1. copy/download the code from GitHub
2. Run deepdrugV.py with a .mol2 file (see Examples)

## Examples

create a 2D image using mol2 file

    python deepdrugV.py --molecule input.mol2 --output output.jpg --dpi integer 
    
![eg_image](https://github.com/rajiv03/DeepDrugV/blob/master/voronoi_2D.jpg=250x250)
