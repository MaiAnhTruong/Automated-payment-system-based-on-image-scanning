# Automated-payment-system-based-on-image-scanning

How does it work?

First, we collect data that is product images from the camera, specifically from the ESP32-CAM. The data will include many angles of the product. Combined with the use of LabelImg to mark the coordinates of the product. Then, we use the augmentation method to diversify the data. So with about 10 initial images, I can generate about 10000 images to provide for the training model. Next, we use the YOLOv8 model, fine-tuned with my data set. On the web side, after having the results from the detection, they will be stored in the database. And from that database, they will be linked to the website to display the product name, quantity, and price. Finally, there will be a QR code to pay for the product.

[This](videooo.mp4) is a video of Product's result:
