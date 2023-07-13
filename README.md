# speed-calculator
/**
 * Calculates the speed given the distance and time.
 * 
 * @param {number} distance - The distance traveled in meters.
 * @param {number} time - The time taken to travel the distance in seconds.
 * @returns {number} The speed in meters per second.
 */
function calculateSpeed(distance, time) {
  try {
    // Check if both arguments are numbers
    if (typeof distance !== 'number' || typeof time !== 'number') {
      throw new TypeError('Both arguments must be numbers');
    }
    
    // Calculate and return the speed
    return distance / time;
  } catch (error) {
    // Log the error
    console.error('Error:', error.message);
    return 0;
  }
}
