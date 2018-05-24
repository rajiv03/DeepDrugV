## DeepDrugV
DeepDrugV constructs the voronoi diagram (VD) of protein binding site/pocket or ligand structure based on the 3D  or 2D coordinate structure. 
3D coordinate will be projected into 2D by perspective projection

    Px= x/1-z 
    Py= y/1-z 

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
    

create a 2D image using protein pocket file in mol2 format

    python deepdrugV.py --molecule 3nbf.mol2 --output voronoi_2D.jpg --dpi 300   
    
## Voronoi image of ATP-binding site protein pocket
 
![eg_image](https://github.com/rajiv03/DeepDrugV/blob/master/voronoi_2D.jpg) 

Heat resistant RNA dependent ATPase (3nbf)
