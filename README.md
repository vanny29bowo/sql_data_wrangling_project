# Data Wrangling and SQL Pacmann — Analisis Dataset Penjualan E-commerce Olist Store

- A. Pada analisis akan digunakan public dataset penjualan yang disediakan oleh Ecommerce asal Brazil yang bernama Olist yang beroperasi di segmen e-commerce namun sebagai perusahaan teknologi SaaS sejak tahun 2015. Analisis ini memiliki objektif untuk menganalisa beberapa point-point berikut:

- 1.Perusahaan ingin mengetahui total penjualan dari tiap kategori produk.
- 2. Perusahaan ingin mengetahui kategori produk yang paling banyak dipesan.
- 3. Perusahaan ingin mengetahui pertumbuhan pemesanan 10 produk yang paling diminati.

- B. Dataset Overview

Namun pada analisis kali ini, hanya akan digunakan 4 tabel sesuai dengan objektif yang sudah ditentukan diawal, berikut tabel yang digunakan:

- a. olist_order_dataset

- order_id : unique identifier of the order
- customer_id : key to the customer dataset. Each order has a unique customer_id
- order_status: reference to the order status
- order_purchase_timestamp: shows the purchase timestamp
- order_approved_at: shows the payment approval timestamp
- order_delivered_carrier_date: shows the order posting timestamp. When it was handled to the logistic partner.
- order_delivered_customer_date: shows the actual order delivery date to the customer
- order_estimated_delivery_date: shows the estimated delivery date that was informed to customer at the purchase moment

- b. olist_order_item_dataset

-  order_id: order unique identifier
- order_item_id: sequential number identifying the number of items included in the same order
- product_id: product unique identifier
- seller_id: seller unique identifier
- shipping_limit_date: shows the seller shipping limit date for handling the order over to the logistic partner
- price: the item price
- freight_value: item freight value item (if an order has more than one time the freight value is splitted between items)

- c. olist_order_products_dataset

- product_id: unique product identifier
- product_category_name: root category of product, in Portuguese
- product_name_lenght: number of characters extracted from the product name
- product_description_lenght: number of characters extracted from the product description
- product_photos_qty: number of product published photos
- product_weight_g: product weight measured in grams
- product_length_cm: product length measured in centimeters
- product_height_cm: product height measured in centimeters
- product_width_cm: product width measured in centimeters

- d. olist_order_product_category_name_transalation

- product_category_name: category name in Portuguese
- product_category_name_english: category name in English

Untuk laporang lengkap terangkum dalam : https://medium.com/@vannybowo/data-wrangling-and-sql-pacmann-analisis-dataset-penjualan-e-commerce-olist-store-3fd004aea75c

