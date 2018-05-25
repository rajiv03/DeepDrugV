## DeepDrugV
DeepDrugV constructs the voronoi diagram (VD) of protein binding site/pocket or ligand structure based on the 3D or 2D coordinate structure. 
                                                         
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
2. If input is a 3D coordinate of protein/ligand, it will be projected to 2D plane employing perspective projection: Px= x/1-z, Py= y/1-z
3. Run deepdrugV.py with a .mol2 file (see Examples)

## Examples

create a 2D image using mol2 file in 2D or 3D format

    python deepdrugV.py -mol input.mol2 -out output.jpg -dpi integer 
    
    -mol stands for the receptor, protein or ligand (MUST BE in a mol2 format)
    -out is the name of the output file (no need to add a .jpg extension)
    -dpi is the desired image quality (eg: 300 dpi in 3.3 x 3.3 = 256 x 256 px)

creating a 2D image of voronoi using protein pocket file in mol2 3D format

    python deepdrugV.py -mol 3nbf.mol2 -out voronoi_2D.jpg -dpi 120   
    
Voronoi image of ATP-binding site protein pocket colored by atom types:
 
![eg_image](https://github.com/rajiv03/DeepDrugV/blob/master/4v94E_voronoi_2D.jpg) 

chaperonin (4v94, chain E)

If you find this tool useful, please cite this paper:

Rajiv Gandhi Govindaraj, Jeffrey Lemoine, Limeng Pu, and Michal Brylinski. "DeepDrugV"
