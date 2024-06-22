# Visual_Image_Search
# Testing

**Run** [Main_Searching_Model_Script.ipynb](https://github.com/Gaurav05082002/Visual_Image_Search/blob/main/Main_Searching_Model_Script.ipynb) **in a notebook environment for seeing completely error-free working demo** Please refer to the [Setting up the environment](https://github.com/Gaurav05082002/Visual_Image_Search?tab=readme-ov-file#setting-up-the-environment) section for detailed setup instructions. 

Currently, our model is trained mostly on women's wear products, so please use traditional wear images like saree, kurta, etc., as input.

## Setting up the environment

**Note:** The model files are large (1.29 GB, 1.30 GB), so please use Google Drive to avoid errors.

1. **Download the Models folder** from [here](https://drive.google.com/drive/folders/1g6j2FTR5WTeDH0iOEcK8AITHLs2nEsGd?usp=drive_link).
2. **Upload it to your Google Drive.**
3. **Mount your Google Drive** in your notebook environment.
4. **Modify the paths for `prediction_by_knn_model.pkl` and `product_maped_to_features` in your code according to your mounted Google Drive.**
5. **Install the required package:**
   pip install ultralytics

**Note:** <u>_When running the cell for the first time, it may take longer. Please wait for some time._</u>

## Solution

### Part 1: Search by Image of Single Product

**Code to retrieve the best similar product link when uploading an image of a single product.** The model performs image scan search and returns a link to a similar product from our demo data on which the model is trained. In the future, the model can be trained on millions of product images to return exact matches.

### Part 2: Shopping from Prime Videos

**When watching Prime Video, clicking the "Shop Now" button sends the video's time frame/screenshot to this model ( written as part 2 in [Main_Searching_Model_Script.ipynb](https://github.com/Gaurav05082002/Visual_Image_Search/blob/main/Main_Searching_Model_Script.ipynb)  file.** The model give cutouts of products in video frame then user select the product cutout which he wants to search, once selected it returns a link to a similar product from our demo data on which the model is trained. In the future, the model can be trained on millions of product images to return exact matches.

## Data Used

### Scraped Data

We scraped data from Amazon products using [amazon_scrapper.ipynb](https://github.com/Gaurav05082002/Visual_Image_Search/blob/main/Data%20Scraper/amazon_scraper.ipynb). The model utilized around 4000+ products from the following categories, each file containing approximately 100 products summed up in `all_combined.csv`:

- `women professional dress`
- `women party wear`
- `women clothing`
- `watches`
- `traditional wear for women`
- `stylish tops for women`
- `saree`
- `salwar suit`
- `lehenga`
- `ghagra`
- `frock for women`
- `formal dress for women`
- `fashionable dresses for women`
- `embroidery kurta`
- `ethnic wear for women`
- `embroidery kura`
- `crop tops`
- `heavy sarees`
- `printed kurtas`
- `red saree`
- `bicycles`
- `bottles`
- `cartoys`
- `comforters`
- `fridges`
- `jackets`
- `tables`
- `televisions`
- `washing machines`

All these data files can be found in the [Scraped Data folder](https://github.com/Gaurav05082002/Visual_Image_Search/tree/main/Data%20Scraper/Scraped%20Data).
