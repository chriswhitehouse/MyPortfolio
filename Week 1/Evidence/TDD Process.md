# [The TDD Process](https://github.com/makersacademy/skills-workshops/blob/master/week-1/TDD_process.md)

Workshop looking at the basics of TDD:

## Why Test?

* To prove that the program is doing what we think it is doing
* Consider any possible scenario
* Considering Edge Cases
* To better understand interdependencies
* To make code more easily changeable
* To help with debugging

## Why write tests first?

* Allow following of client brief more closely
* You only write code to pass your tests
* Tests are based on requirements
* Helps to avoid extraneous code

##TDD Steps:

* User Stories
* Plan
* Test
    * Red
    * Green
    * Refactor
* Repeat

---

## Other things learnt:

* Respec methods can looked up in relish. In particular the matchers.
* can type `irb -r filepath` the -r means require
* Test it exists
* Then test behaviour
* when testing objects don't need quotes or colons. When testing methods, use colons.
* e.g. the first block tests the instance of Dice object the second tests the dice instance responds to the roll method:

      describe Dice do
       it 'allows the user to create an instance of Dice' do
         dice = Dice.new
         expect(dice).to be_instance_of Dice
       end

       it "should respond to roll " do
         dice = Dice.new
         expect(dice).to respond_to :roll
       end
      end
