<h1>Blog Website</h1>
<p>This is a website for creating and viewing posts from other people. It has functionality for creating, updating, and deleting posts. You can also view posts by user. 
  The website also authenticates users, including password resets if needed. Users can also personalize their account by changing usernames, emails as well as profile pictures. 
  
  The site was written mostly in Python using the Flask framework. It also uses SQLite for the database, and some HTML and Bootstrap CSS for styling elements. 
  This project was inspired by the Flask series by Corey Schafer. 
</p>

<h2>Running the site</h2>
<p>In the future, I may deploy the site, but for now you have to local host it. To use it: simply clone this repository using 
  <br><code>git clone https://github.com/tyler-ingram/BlogWebsite.git</code><br>and install these packages using pip.<br>
<code>
pip install flask-login
pip install flask-bcrypt
pip install FLASK-WTF
pip install Flask-SQLAlchemy
pip install flask
pip install Pillow
pip install flask-mail
</code>
  <br>
  Then set your environment variables in your operating system for the variables in config.py. Alternatively, if security is not a concern, you can hard-code them in the same file.<br>If you want to use a database instance already created and populated, set <code>SQLALCHEMY_DATABASE_URI = sqlite:///path\to\site.db</code> in config.py or as an environment variable. 
  If you want to make your own database instance, create it at the command line using<br>
<code>
python 
from flaskblog import create_app, db
app.app_context().push()
db.create_all()
</code>
The posts will be empty because you created your own db instance, but you can populate it after making an account. 
Now you should be able to run the program using <br><code>python run.py</code>

</p>
