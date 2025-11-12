# JS Snow Flakes

This script can be inserted into an HTML header to add a snowfall effect to any website. The effect is highly configurable by using simple variables.

## Integration

To integrate the script into your HTML file, copy and paste one of the following tags into an HTML header:

JavaScript version:
```html
<script src="https://cdn.jsdelivr.net/gh/omeyenburg/js-snow-flakes@main/snowflakes.min.js"></script>
```

CSS version:
```html
<script src="https://cdn.jsdelivr.net/gh/omeyenburg/js-snow-flakes@main/snowflakes_css.min.js"></script>
```

If you prefer to modify the variables, add another script tag containing your adjustments.
Refer to the list of available variables below for customization options.
Here is an example for the usage with adjustments to `SNOWFLAKE_SPEED` and `SNOWFLAKE_NUMBER`.

```html
<script src="https://cdn.jsdelivr.net/gh/omeyenburg/js-snow-flakes@main/snowflakes.min.js"></script>
<script>
    SNOWFLAKE_SPEED = 0.5;
    SNOWFLAKE_NUMBER = 30;
</script>
```

In case you encounter performance issues, consider using an alternative version that uses CSS for animations. You might also prefer to use it, as it is less subsceptible to bugs. Include the script as follows:

```html
<script src="https://cdn.jsdelivr.net/gh/omeyenburg/js-snow-flakes@main/snowflakes_css.min.js"></script>
```

Feel free to experiment with other variables to achieve the desired visual effect on your website!  

## Example
You can find an example [here](example.html).

## Customizable variables

### SNOWFLAKE_START_DATE and SNOWFLAKE_END_DATE
Set the time range during which the snowflake effect is active. The end date is exclusive. By default the effect will be effect active all year, but you can configure it to only be active during Christmas. The date format consists of the month followed by a decimal point and the day. Ensure single-digit days have leading zeros. Months should not have leading zeros.  
Default:  
`SNOWFLAKE_SET_DATE = false;`  
`SNOWFLAKE_START_DATE = 12.22;`  
`SNOWFLAKE_END_DATE = 12.26;`

### SNOWFLAKE_SPEED
Determine the average downward velocity for each snowflake.  
Default:  
`SNOWFLAKE_SPEED = 1;`

### SNOWFLAKE_SPEED_DIVERGENCE
Specify the range for the speed of the snowflakes as a divergence.  
Default:  
`SNOWFLAKE_SPEED_DIVERGENCE = 3;`

### SNOWFLAKE_MIN_SIZE and SNOWFLAKE_MAX_SIZE
Set the range of random sizes in pixels for each snowflake.  
Default:  
`SNOWFLAKE_MIN_SIZE = 5;`  
`SNOWFLAKE_MAX_SIZE = 15;`

### SNOWFLAKE_ROTATION_SPEED
Control the rotation speed of snowflakes in degrees per second. This option is not supported by the CSS version.  
Default:  
`SNOWFLAKE_ROTATION_SPEED = 25;`

### SNOWFLAKE_NUMBER
Set the total count of snowflakes spawned at the beginning.  
Default:  
`SNOWFLAKE_NUMBER = 15;`

### SNOWFLAKE_CENTER_REDUCTION
Reduce the spawning of snowflakes in the center of the screen.  
Default:  
`SNOWFLAKE_CENTER_REDUCTION = true;`

### SNOWFLAKE_COLORS
An array containing possible colors from which the color for each new snowflake is randomly chosen.  
Default:  
`SNOWFLAKE_COLORS = ["#dddddd", "#eeeeee", "#ffffff"];`

### SNOWFLAKE_SYMBOLS
Each newly spawned snowflake is assigned a random symbol from this array.  
Default:  
`SNOWFLAKE_SYMBOLS = ["❅", "❆", "*", "●"];`

### SNOWFLAKE_SHADOW
Enable a slight shadow behind snowflakes.  
Default:  
`SNOWFLAKE_SHADOW = true;`

### SNOWFLAKE_SHADOW_COLOR
Set the color of shadows behind snowflakes when shadows are enabled.  
Default:  
`SNOWFLAKE_SHADOW_COLOR = #000000;`

### SNOWFLAKE_SPAWN_ON_SCREEN
Spawn snowflakes on the screen instead of above it when the site loads. This option is not supported by the CSS version.  
Default:  
`SNOWFLAKE_SPAWN_ON_SCREEN = false;`
