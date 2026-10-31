# Tower Ops

The operator console for **Humanoid Delivery**: the software layer that runs robots inside a residential high-rise. Proof of concept with simulated data.

A simulated 30-floor Miami tower with one robot on shift:

- **Tasks come in** from couriers (the desk stickers the bag with the unit number), sidewalk robots, the package room and scheduled trash-room runs.
- **The robot runs on its own:** it reads the unit sticker, loads up to 10 orders, taps its own building fob, presses the elevator button and leaves each order at the door with a photo.
- **A human only when it's hard:** at a heavy fire door the robot asks for help; if nobody takes over within 70 seconds, an offshore operator does. Every takeover is logged as training data, so the next one needs no human.
- **Shift metrics:** tasks completed, front-desk calls avoided, minutes from lobby to door, operator takeovers.

Built as a single self-contained HTML page: an SVG building section, a robot state machine that plans each task as a sequence of actions, a live task queue, random door-help events and a remote-takeover flow.

Part of [Humanoid Delivery](https://github.com/ziurr), the access layer that lets robots work inside buildings. Starting in Brickell, Edgewater and Midtown Miami.
