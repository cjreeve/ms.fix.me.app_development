**Comments by cjreeve**

- update

I just uploaded an example of the kind of programming work I have been doing to https://github.com/cjreeve/portfolio

I'm sorry it is a bit messy - I seem to have misplaced the final version. If there is time, I shall start working through the RoR tutorial and add further examples to the portfolio. 

C



------------------------------------------------
Dear Peter,

Thank you for the opportunity for me to take part in this Ruby on Rails development test. I am an experimental particle physicist by training but am keen start a career in web development. My previous programming experience is in C++, Matlab and a little python, and this task will is the first time I have looked at Ruby on Rails and Ruby code.

I have enjoyed the challenge. I regret that I have run out of time so that I cannot make any impressive changes. Much of my time was taken up with setting up the app on my computer. I initially attempted this on my Mac but ran into problems updating Ruby1.8 to 1.9. I eventually had it running on my Linux computer, but being the first time at setting up a server, this also took a little time.

I am becoming familiar with the Rails folder structure but it would be ideal if I spent some time working through the online tutorial manual before attempting major changes.
Currently I have only played with a little CSS formatting and indicated a couple of ideas I was thinking of implementing.

I would be grateful if you can offer me the opportunity to come in for a chat.

Best regards,

Christopher





--------------------------

**MsFixMeApp** is a basic Rails 3 app that we'd like you to make some changes to.

The application 'approximates' an eCommerce site. It shows categories and products on the 'front end' and allows
the site owner to update the descriptions etc in the 'back end'

You can't add anything to your basket / cart - there isn't an order or basket model. Basically all that you can do at the 
moment is browse around the site.

We just want you to add something (or fix something) to the application and show us what you did and then explain why / how.

Requirements
===
- Ruby 1.9.3
- Gems are listed in the Gemfile

Getting the application running
===

Create a database called 'ms.fix.me.app_development'

Then either create a user with write permission to the above database called:

msdev
password

Or, update the database.yml with user credentials that can connect

CD to your local copy

```bash
bundle install
bundle exec rake db:setup
rails s
```

Go to localhost:3000 and you should then see the public web site / front end
Go to localhost:3000/administration for the administration console

Things To Do
===

Feel free to make whatever changes you like. Just push them back to your Git Hub branch so that we can have a look
and we'll chat about them when we meet with you. What we're after is seeing if you can look at an app, work out how it works and
then make some changes to it. As long as your change adds (or fixes) something and you can justify and discuss what you did,
then that will be great. No need to go overboard :)

Here are some suggested tasks, however feel free to come up with your own:

- http://localhost:3000/administration/products shows a list of all the'published' products, add a way of showing a list of products
with other published statuses (draft, submitted, archived, deleted)
- Add a way that we can 'bulk archive' selected products on this page: http://localhost:3000/administration/products
- Add a way of inserting a chunk of text on the home page that an administrator can edit
- Add a way of creating a free text page, eg a contact us page that can be edited in administration
- Add the price for each variant on the public product page
- Add a price range for all variants for each product in the 'product_tile' (ignore currency symbols)
- Add a way of uploading an image to a product or category
- Are there any performance issues that need to be addressed, especially if the site had 10,000's of products - how can this be resolved?
- Make the administration pages look better
- Add a login page for administration pages
- Show which categories a product belongs to (think about published statuses)
- Show which products belong to a category (think about published statuses)
- Add a way to add a product to a category - AJAX would be nice, but not necessary
- Add a way to create a new variant for a product
- Add a way to edit a variant on a product page
