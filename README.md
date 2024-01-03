# -from flask import Flask, render_template

app = Flask(__name__)

# Define routes for different pages
@app.route('/')
def home():
    # Render the homepage template
    return render_template('index.html')

@app.route('/products')
def products():
    # Render the products page template
    return render_template('products.html')

# Other routes for user authentication, checkout, etc.

if __name__ == '__main__':
    app.run(debug=True)
