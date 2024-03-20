# Carousel Widget

The `Carousel` widget is a Flutter widget that provides a customizable carousel view for displaying images or Lottie animations in your Flutter applications.

## Constructor

### `Carousel`

- `carouselAssets`: A list of `CarouselAsset` objects representing the assets to be displayed in the carousel.
- `activeColor`: The color of the active indicator circle.
- `inactiveColor`: The color of the inactive indicator circles.
- `backgroundColor`: The background color of the carousel widget.
- `indicatorCircleSize`: The size of the indicator circles.
- `indicatorCirclePadding`: The padding around the indicator circles.
- `scrollingTime`: The time interval (in seconds) for automatic scrolling to the next page.

## Properties

### `activeColor`

- Type: `Color`
- Description: The color of the active indicator circle.

### `inactiveColor`

- Type: `Color`
- Description: The color of the inactive indicator circles.

### `carouselAssets`

- Type: `List<CarouselAsset>`
- Description: A list of `CarouselAsset` objects representing the assets to be displayed in the carousel.

### `backgroundColor`

- Type: `Color`
- Description: The background color of the carousel widget.

### `indicatorCircleSize`

- Type: `double`
- Description: The size of the indicator circles.

### `indicatorCirclePadding`

- Type: `double`
- Description: The padding around the indicator circles.

### `scrollingTime`

- Type: `int`
- Description: The time interval (in seconds) for automatic scrolling to the next page.

## Methods

### `_nextPage()`

- Description: Moves to the next page in the carousel.

### `_previousPage()`

- Description: Moves to the previous page in the carousel.

### `_showInitialPage({required Duration duration})`

- Description: Shows the initial page of the carousel.

### `_restartLottieAnimation()`

- Description: Restarts the Lottie animation if the current index corresponds to a Lottie asset.

### `_stopTimer()`

- Description: Stops the timer used for automatic scrolling.

## Usage

To use the `Carousel` widget, create an instance of it and provide the necessary parameters:

```dart
Carousel(
  carouselAssets: [
    CarouselAsset(id: '1', path: 'assets/animation1.json', type: CarouselType.lottie),
    CarouselAsset(id: '2', path: 'assets/image1.png', type: CarouselType.image),
    // Add more CarouselAsset objects as needed
  ],
  activeColor: Colors.blue,
  inactiveColor: Colors.grey,
  backgroundColor: Colors.white,
  indicatorCircleSize: 8.0,
  indicatorCirclePadding: 4.0,
  scrollingTime: 3, // 3 seconds scrolling time
)
