# Plan of action

As we didn't get to finish coding Snake, I've decided to give you a bit more guidance on the approach you might want to take in continuing with your implementation. This is all off the top of my head, and, as such, is more of a rough guide than gospel. So be prepared to do some additional thinking, stuggling, and looking stuff up in the Ruby and Gosu documentation.

When doing mentally exhausting tasks, something that helps me is to have a pre-defined amount of struggle time on any one part of the problem (say 15mins, before reaching for the answer). Consistently struggling for longer is mentally exhausting. Be kind to your confidence and enthusiasm: they are important resources, don't throw too much at them. 

### Approaches

These can also be thought of as progressions. A great way to learn would be to do Normal, then Hard, then Insane. Or, alternatively, pick one, then move on to another project. 

**Normal**

Try and understand what each line in the completed version is doing (get it [here](https://github.com/nazwhale/ruby-snake)). Us humans learn better by doing, so code along in your own text-editor, following my plan of attack (Let's get down to business). If you had never coded before and you can get to the point where you understand most of the completed version, you are doing phenomenally well.

**Hard**

Instead you might prefer to try and challenge yourself by tackling it without looking at the completed version (still very hard if you're new to programming!) and just using my steps.

**Insane**

Designing a program is a skill that we didn't get to touch on, and you might find that you'd rather have a crack at plotting your own plan of action before looking at mine.

If so, great. My advice would be to diagram lots, and be "Agile" in your approach. A simple definition of Agile is that it means planning to re-plan at regular intervals, being adaptive, not hanging on to old ideas. You'll come to learn that, in the end, a piece of software never quite looks how you thought it would at the start. So have the peace of mind to take a step back and re-evaluate your approach as often as you need to.

### [Let's get down to business](https://www.youtube.com/watch?v=ZSS5dEeMX64)

That said, if you simply want to get something working and then play around, here's some steps you might like to take:

1) Make the Game Window ◻

2) Make an Apple 🍎
- update `apple.rb` with a `draw` method using the `@window.draw_quad`, `x` and `y` coordinate properties
- don't forget to draw it in your Game Window

3) Draw a Segment ✍
- same steps apply as above

4) Turn your Segment into a 1 segment Snake ✨
- create an `@segments` array
- push the head into it
- don't forget to draw it in the Game Window

5) Move your 1 Segment Snake with the arrow keys ⬆
- create a `@direction` variable in your Snake class
- in Game Window, create an `update` method (refer to the Gosu documentation to understand what `update` is for). In `update`, add some logic so that if a button is pressed on the keyboard (again, see Gosu docs), `@snake.direction` changes
- make a method to define what how a "right" or "left" or "up" or "down" value in the `@direction` variable should affect the `@x` and `@y` properties of your Snake
- make an `update_position` method, which adds the latest segment to the start of a snake, and removes the oldest segment from the end of the snake
- run the program and play with your baby Snake!

6) Eat some apples 🍴
- create an `ate_apple?` method in Snake, with appropriate logic to return `true` if the head of the Snake is on the same part of the window as an Apple
- create a `@score` property in Game Window, initialized at 0
- update the `update` method in Game Window to add some points to `@score`, increase the length of the snake, and generate a new apple, everytime `@snake.ate_apple?` is true

7) Introduce speed 💨
- create a `@speed` variable within the Snake class
- increase `@speed` every time an apple is eaten, or, if you prefer, every time `@score` increases by a certain amount (or a mixture of the two)

8) Show the score 💯

9) Lose conditions in Snake class 💀
- `outside_bounds?`
- `hit_self?`

### [It gets easier](https://www.youtube.com/watch?v=R2_Mn-qRKjA)

And there's almost certainly more. Try and figure out how you'd design any additional functionality, or feel free to refer to the completed version and see what's missing. If you've come this far, you're doing great.

Keep testing your work by running `ruby play.rb` while making improvements, keep decipering those error messages, and keep reminding yourself that you're better at this than you were yesterday. 

Once you're content, on with the [challenges!](https://github.com/nazwhale/snakers-academy/blob/master/challenges.md) 🎉
