# ShoppingBuddy
Sooner or later, we all find ourselves choosing clothes from an online shop, but navigating these sites to find what best matches our tastes is often a frustrating and tedious task.   
It would be much better to have a friend who performs an initial screening for us, suggesting items that might align with our preferences, directly from the provided web page.
  
ShoppingBuddy is a personalized recommendation system based on ResNet50, developed to provide quick insights into products available on a fashion website according to your preferences.  
The model is trained by assigning a fit-rate [0 to 1] to each item. Images are processed in black and white to focus on the fit and cut of the garment, rather than the color, which often depends on the rest of the outfit being created.

## Get Started

To use the system, you need to:

0. **Set All**: Run all [dev] cells
   >Set environment [dev]  
    Import packages [dev]  
    Code block [dev]
1. **Create Your Dataset**: Build a labeled dataset with a fit-rate for each item in the provided URLs (more items, more accuracy).
   >_train_urls = [url_1, url_2, url_3, url_4, url_5, url_6]_  
    _build_dataset(train_urls)_
2. **Train the Model**: Train the ResNet50 model with the created dataset.  
   > _train_model()_
3. **Provide URL for Predictions**: Once trained, the model is ready to make predictions on products in the URL.
   >_pred_url = ['url_7']_  
    _use_model(pred_url, lang='en')_

**Note**: Currently, the system supports only Mango and Mango Outlet websites.

