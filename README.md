# E06a-Bullets
Playing with bullet sprites:

It's narwhals vs. penguins(?)! These natural enemies are locked in a battle; who will survive?

I have given you the beginnings of a shooter game. At a minimum, you will need to generate a bullet when the mouse button is clicked (line 95), and then detect a collsion with a penguin (line 76), decrease its health, check if it dies, and increase the player's score.

In main1.py you will find the code that allows the narwhal to shoot bulletts at the penguins and kill them and earn points. 

For extra credit, end the game when all the penguins have been killed.

I will award significant extra credit if you subsequently create a main2.py, using the same framework, that allows the penguins to fire back. I have included a bullet_enemy.png asset for that purpose. Even more points will be awarded if you include explosions and/or damage indicators.

To get you started, this is how I generated a new bullet:

```
    x = self.player.center_x
    y = self.player.center_y + 15
    bullet = Bullet((x,y),(0,10),BULLET_DAMAGE)
    self.bullet_list.append(bullet)
```

The arcade.check_for_collision_with_list(sprite, spriteList) method takes a sprite and a spriteList and returns a list of any elements from spriteList that are currently colliding with sprite.

self.player.kill() will remove the player sprite. .kill() can be (similarly) used to remove any sprite.

As always, let me know if you have any questions.