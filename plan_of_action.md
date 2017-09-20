# Plan of action

As we didn't get to finish coding Snake, I've decided to give you a bit more guidance on the approach you might want to take in continuing with your implementation. This is all off the top of my head, so be prepared to do some thinking, stuggling, and looking stuff up in the Ruby and Gosu documentation.

You might like to do this while referring to the completed version of snake open in another window (get it [here](https://github.com/nazwhale/ruby-snake)), or try and challenge yourself by tackling it without looking (still very hard if you're new to programming!).

Designing a program is a skill that we didn't get to touch on, and you might find that you'd rather have a crack at planning your own plan of action before looking at mine.

If so, great. My advice would be to diagram lots, and be "Agile" in your approach, meaning that you plan to re-plan. You'll come to learn that, in the end, a piece of software never quite looks how you planned it would at the start. So have the piece of mind to take a step back and re-evaluate your approach as often as you need to.

That said, if you simply want to get something working and then play around, here's some steps you might like to take:

1) Make the Game Window

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
- initial `@speed` variable within the Snake class
- increase `@speed` every time an apple is eaten, or, if you prefer, every time `@score` increases by a certain amount

8) Show the score 💯

9) Lose conditions in Snake class 💀
- `outside_bounds?`
- `hit_self?`

And there's probably a bunch of other stuff I've forgotten. Keep testing your work by running `ruby play.rb` and making improvement.

Once you're done, on with the [challenges!](https://github.com/nazwhale/snakers-academy/blob/master/challenges.md) 🎉
