# Dense Depth model with Custom Dataset
### 1) Link to Custom Dataset: 

https://drive.google.com/drive/folders/1RbJHVxo91jhekv3_E9GZvujUDNDaxFQu

### Folder Structure

:small_orange_diamond:**Background**: Contains 100 background images (bg1 to bg100)

:small_orange_diamond:**Foreground**: Contains 100 foreground images (fg_bg1 to fg_bg100)

:small_orange_diamond:**Mask**: Contains 100 mask of foreground images (mask1 to mask100)

:small_orange_diamond:**Dataset**: Contains 5 zip files (data_Part1.zip to data_Part5.zip)

Each .zip file contains 80k fg-bg images, 80k fg-bg masks and 80k depth maps (5 zip files x 80k images = 400k images each):

- Fg-Bg: Contains images where foreground is overlapped on background (fg-bg1 to fg-bg400000)

- Fg-Bg-Mask: Contains mask images where foreground is overlapped on background (fg-bg-mask1 to fg-bg-mask400000)

- Depth: Contains depth map images generated from Dense Depth model (depth1 to depth400000)

- labels.txt: Containing paths to all folders

**Structure of any one zip folder**

├── Dataset

   ├── data_Part1.zip
  
    ├── Fg-Bg
    
    |   ├── fg-bg1.jpg
    
    |   ├── fg-bg2.jpg
    
    |   ├── ...
    
    |   └── fg-bg80000.jpg
    
    ├── Fg-Bg-Mask
    
    |   ├── fg-bg-mask1.jpg
    
    |   ├── fg-bg-mask2.jpg
    
    |   ├── ...
    
    |   └── fg-bg-mask80000.jpg
    
    ├── Depth
    
    |   ├── depth1.jpg
    
    |   ├── depth2.jpg
    
    |   ├── ...
    
    |   └── depth80000.jpg
    
    ├── labels.txt
   
   
### 2) Kinds of images

:large_blue_circle:**Background**

- Image Description: **Living Rooms** :house:
- Image Size: 224x224
- Image Extension: .jpeg
- Total number of images: 100

:large_blue_circle:**Foreground**

- Image Description: **Humans** :couple:
- Image Extension: .png
- Total number of images: 100

:large_blue_circle:**Mask**

- These are foreground masks generated :black_square_button:
- Image Extension: .jpg
- Total number of images: 100

:large_blue_circle:**Fg-Bg** 

- Image Description: Humans overlapped on living room images :city_sunset:
- Image Size: 224x224
- Image Extension: .jpeg
- Total number of images: 4,00,000

:large_blue_circle:**Fg-Bg-Mask** 

- These are foreground-background masks generated :black_square_button:
- Image Extension: .jpg
- Total number of images: 4,00,000

:large_blue_circle:**Depth** 

- These are depth maps generated from dense depth model :ghost:
- Image Extension: .jpg
- Total number of images: 4,00,000


### 3) Total number of images of each kind

:small_red_triangle_down:**Background** - 100

:small_red_triangle_down:**Foreground** - 100

:small_red_triangle_down:**Foreground-Mask** - 100

:small_red_triangle_down:**Foreground-Background** - 4,00,000

:small_red_triangle_down:**Foreground-Background-Mask** - 4,00,000

:small_red_triangle_down:**Depth Maps** - 4,00,000

### 4) Total size of dataset


### 5) Mean and STD values:

**Fg-Bg:**
- Mean: [0.65830478, 0.61511271, 0.5740604 ]
- STD: [0.24408717, 0.2542491 , 0.26870159]

**Fg-Bg-Mask:**
- Mean: [0.04608837, 0.04608837, 0.04608837]
- STD: [0.20544916, 0.20544916, 0.20544916]

**Depth:**
- Mean: [0.50911522, 0.50911522, 0.50911522]
- STD: [0.28174302, 0.28174302, 0.28174302]

### 6) How the images look like?

:camera: **Background**

:camera: **Foreground**

:camera: **Foreground-Mask**

:camera: **Foreground-Background**

:camera: **Foreground-Background-Mask**

:camera: **Depth Images**

### 7) Creation of Dataset

We are a team of 5 members and we divided the work among us, equally.

**Background**
