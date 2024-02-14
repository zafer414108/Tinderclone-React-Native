# Tinderclone-React-Native
# State:

# hearts: An array in the component's state to keep track of individual hearts.
# height: Height of the container layout, used for positioning hearts.
# Methods:

createHeart(index): Creates an object representing a heart with a unique id and a random right value.
removeHeart(id): Removes a heart from the state based on its id.
# Lifecycle Methods:

UNSAFE_componentWillUpdate(nextProps): Adds new hearts when the count prop is updated.
Render:

Renders a container (View) with a background color and nested AnimatedShape components representing the floating hearts.
# AnimatedShape Component:
State:

position: An animated value controlling the vertical position of the heart.
shapeHeight: Height of the heart shape.
enabled: A boolean indicating whether animations are enabled.
animationsReady: A boolean indicating whether animations are ready.
# Lifecycle Methods:

componentDidMount(): Initializes and starts the animations when the component mounts.
handleOnLayout(e): Sets up various animations based on the layout height of the heart shape.
# Animation Styles:

Uses interpolation to create animated transformations (translation, scale, rotation, and opacity) based on the heart's position.
Render:

Renders an animated wrapper (Animated.View) around the provided children.
# HeartShape:
It's assumed that the HeartShape component is imported but not provided in the code snippet. This component likely represents the visual representation of a heart.
# Styles:
Styles for the container and the shape wrapper.
# Helpers:
getRandomNumber(min, max): A helper function that generates a random number between min and max.
# PropTypes:
PropTypes are defined for both FloatingHearts and AnimatedShape components.
# Exports:
The FloatingHearts component is exported as the default export.
Screen Gif :


https://github.com/zafer414108/Tinderclone-React-Native/assets/147662873/fd287c9d-bb53-495a-8e55-09513a53c59e

