# ShoppingBuddy

ShoppingBuddy is a personalized recommendation system based on ResNet50, developed to provide quick insights into products available on a fashion website according to your preferences.  
The model is trained by assigning a fit-rate to each item. Images are processed in black and white to focus on the fit and cut of the garment, rather than the color, which often depends on the rest of the outfit being created.

## Using the System

To use the system, you need to:

1. **Create Your Dataset**: Build a labeled dataset with a fit-rate for each item.
2. **Train the Model**: Train the ResNet50 model using the created dataset.
3. **Provide URLs for Predictions**: Once trained, the model is ready to make predictions on products provided via URLs.

**Note**: Currently, the system supports only Mango and Mango Outlet websites.

