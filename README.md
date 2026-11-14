# MG6

1. The entire loop happens inside one Update() or one frame. Usually, long loops don't really matter as much nowadays, since our devices have such high computing power. But say if it were a really long and complex loop, the game would lag and have slower frames yes.

2. Our player can get stuck inside platforms, which then needs us to jump out. But if you go too high you can't get down. The getting stuck happens because collisions are disabled when the linearvelocity y is positive or going up, which then if it goes to 0 from gravity as we are inside a platform, collisions turn on, and hence, we are stuck.