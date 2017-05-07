# Make Ruby Great Again
## Rails Conf 2016 
- viewed on appleTV - vimeo app
- Justin Searls: @searls 
- works for test double 
- http://blog.testdouble.com/posts/2016-05-09-make-ruby-great-again.html
- giving talk in place of @samphippen, a part of rspec core

### Minitest Is Not Better than RSpec

### RSpec + Rails 5
- Will RSpec just work w/ Rails5? no! 
- Hug a maintainer - lots of work to support Rails5
- Rspec 3.5.0
- Are functional/controller tests really deprecated? Yes!
  - Controller tests -- somewhere between full stack tests & unit tests --> hard to explain, not terribly helpful
  - Faster at run-time, slower at fix-time 
  - Instead of writing controller specs, write full stack feature specs, or request specs, or nothing 
  - full stack tests: untestabe ways things can break 
  - unit tests: unclear reasons why tests might fail
  - controller specs: not terribly helpful, imples an API request is being made-- just invokes the controller methods, does not address middleware, etc. instead, look @ integration testing to ensure 
  - `gem 'rails-controller-testing'` if you still want to write controller specs
  - request specs are honest versions of controller tests -- exercise routes, middleware, views, you can access response.body
- Does RSpec offer anything to test Action Cable? No.  Test through the browser now. 

### Why are you here? 
- 3 theories: 
 - "how do i test action cable?"
 - "i am not happy with my test suite?"
 - "i'm new here"
- Searching for a tool is easier than introspection
- keys to happiness
  - 1. tools
  - 2. how we use the tools
- tools matter, they aren't everything. tools prompt behavior. some enable bad habits.
- `rspec-rails` -> bad approach. enables bad habits. not a lot of critical thought behind this. 
  - just use feature specs, model specs, plain ol ruby -> plain ol rspec 
  - the 7 layers are redundant, not super helpful
- RSpec
  - assertions guide test names
  - very DRY, lots of symmetry 
  - makes intenion more clear ` let(:user) {User.new}` vs `let!(:user) {User.create}` 
    - let! should be used to draw attention to side effects 
  - rspec reduces friction, cli helps you focus
  - built in reporters
  - fosters empathy 
  - asks intent 
  - DSL (domain specific language) shifts perspective 
  - minitest - not a lot of opinions
    - different priorities: fast, mean lean testing machine 
    - Rspec is more full featured
    - zeitgeist: minitest is really hot right now. DHH likes it. Ppl think RSpec is bloated, verbose, etc. 
  - Learn a lot discussing RSpec with past teams 
  - RSpec takes longer to learn, but you do learn more about design, etc. 
- http://is.gd/stophate 

### RSpec + Rails 5 
- Assume the author is smart
- Check out Sam's blogpost 
- safe talk... but comfort should scare us
- comfort can breed complacency 
- minitest buzzy 
- rails jobs are on the decline 
- Node.js is buzzy - 900% year over year growth
- challenge: disown comfort || see ruby jobs dry up
- why did our community think RubyTogether was necessary? 
- google isn't going to drop go unless htey feel like it...
- js cannot die b/c multiple vendors have staked their ventures on it 
- rspec is mature -- mostly done (like ruby, rails, bundler)
- maintaining rspec/rails/ruby/bundler doesn't get you famous 
- ruby needs energy & funding 
- entrepreneurs are being sold MongoDB, Express.js, Angular.js, Node.js (MEAN sack); Node & React; Ruby & Rails
  - there aren't enough rubyists, rails doesn't scale, ruby is slow, rubyists are too $$$$
- but rails is still the best choice for so many applications. we just stopped selling it b/c it isnt new & shiny 
- our dilemma: ruby is not new, ruby is still good, what do we do to keep it relevant? 
  - it is ok for tools to be "complete"
- We need to start thinking more about how to use the tools -- think more critically about human issues, design, testing, etc. 
- tell stories that help people solve problems
- if you love ruby, tell your story in ruby
- most people who have made ruby great have moved on
- keeping ruby relevant is our job 

