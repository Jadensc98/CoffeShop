# Making CoffeeShop

first generate a rails project and set it up for git and github

````bash
rails new coffee_shop
cd coffee_shop 
subl . 
git init 
git add . 
git commit -m "first commit"
git remote add origin (link)
git push origin master 
````

Second: add welcme page

```bash
rails g controller Welcome index 
````

In config/routes.rb alter index route to 

`route "welcome#index"`
In app/views/welcome/index 

````html 
<h1>Welcome to JavaCoffeeShop</h1>
<p>Mocha, single shot flavour milk, organic black, lungo instant redeye plunger pot breve. Et crema cortado bar aromatic pumpkin spice cortado variety percolator. Sweet, bar organic eu strong caffeine body.</p>

<p>Macchiato, cup, caffeine brewed in ut brewed froth mazagran. That froth, grounds, turkish, trifecta, filter dripper acerbic french press aged. A skinny cortado, doppio, americano et beans caffeine redeye decaffeinated.Mocha, single shot flavour milk, organic black, lungo instant redeye plunger pot breve. Et crema cortado bar aromatic pumpkin spice cortado variety percolator. Sweet, bar organic eu strong caffeine body.</p>

<p>Macchiato, cup, caffeine brewed in ut brewed froth mazagran. That froth, grounds, turkish, trifecta, filter dripper acerbic french press aged. A skinny cortado, doppio, americano et beans caffeine redeye decaffeinated.Mocha, single shot flavour milk, organic black, lungo instant redeye plunger pot breve. Et crema cortado bar aromatic pumpkin spice cortado variety percolator. Sweet, bar organic eu strong caffeine body.</p>

<p>Macchiato, cup, caffeine brewed in ut brewed froth mazagran. That froth, grounds, turkish, trifecta, filter dripper acerbic french press aged. A skinny cortado, doppio, americano et beans caffeine redeye decaffeinated.Mocha, single shot flavour milk, organic black, lungo instant redeye plunger pot breve. Et crema cortado bar aromatic pumpkin spice cortado variety percolator. Sweet, bar organic eu strong caffeine body.</p>

<p>Macchiato, cup, caffeine brewed in ut brewed froth mazagran. That froth, grounds, turkish, trifecta, filter dripper acerbic french press aged. A skinny cortado, doppio, americano et beans caffeine redeye decaffeinated.</p>
````

Save to git and github in terminal 

````bash
git add .
git commit -m "added landing page"
git push origin master 
````
### Third: Add Drinks 

````bash 
rails g scaffold Drink name:string size:integer  price:decimal
rails db:migrate 
rails s 
````
In browser, go to http://localhost:3000/drinks to add several drinks to database. 

Save to git and github in terminal 

````bash
git add .
git commit -m "added drinks scaffold"
git push origin master 
````

