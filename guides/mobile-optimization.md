# Mobile Optimization for Unity Game Templates

A Unity game template may run smoothly in the Editor while still performing poorly on mobile devices.

Optimization should be part of the reskin and publishing workflow, especially when targeting a wide range of Android and iOS devices.

## 1. Test on Real Devices

Do not rely only on Unity Editor performance.

Test the game on:

- Low-end Android devices
- Mid-range Android devices
- Target iOS devices when applicable

Measure performance during actual gameplay rather than only at the main menu.

## 2. Optimize Textures

Large textures can increase memory usage and build size.

Review:

- Texture resolution
- Max Size
- Compression settings
- Texture format
- Mipmap requirements

Use the smallest texture resolution that provides acceptable visual quality.

## 3. Reduce Draw Calls

Too many draw calls can reduce rendering performance.

Consider:

- Sharing materials where appropriate
- Using texture atlases
- Static batching
- Dynamic batching where appropriate
- Reducing unnecessary objects

Use Unity profiling tools to identify rendering bottlenecks.

## 4. Optimize 3D Models

Review the complexity of models used in the game.

Check:

- Polygon count
- Mesh complexity
- Number of objects
- Level-of-detail requirements

Use simpler models where visual quality allows.

## 5. Control Particle Effects

Particle systems can become expensive when many particles are active simultaneously.

Review:

- Particle count
- Emission rate
- Particle lifetime
- Overdraw
- Particle textures

Avoid unnecessary full-screen particle effects.

## 6. Optimize Physics

Physics calculations can become expensive when many objects interact.

Check:

- Rigidbody count
- Collider complexity
- Collision layers
- Fixed timestep
- Unnecessary physics calculations

Disable physics components when they are no longer required.

## 7. Optimize Audio

Review:

- Audio compression
- Sample rate
- Clip length
- Streaming settings
- Duplicate audio files

Use appropriate compression settings for mobile games.

## 8. Reduce Memory Usage

Monitor memory during gameplay.

Look for:

- Large textures
- Unused assets
- Duplicate assets
- Large audio files
- Unnecessary instantiated objects

Remove assets and systems that are not required.

## 9. Optimize UI

Complex UI can increase rendering and layout costs.

Review:

- Canvas structure
- UI elements
- Layout groups
- Animations
- Canvas rebuilding
- Excessive transparency

Keep frequently changing UI elements organized separately where appropriate.

## 10. Optimize Asset Loading

Avoid loading everything at startup if it is not required.

Consider:

- Loading assets when needed
- Unloading unused assets
- Addressables where appropriate
- Reducing initial scene complexity

Faster loading can improve the overall mobile experience.

## 11. Reduce Build Size

Review the final build for unnecessary content.

Check:

- Unused assets
- Duplicate resources
- Large textures
- Audio files
- Unnecessary packages
- Development-only content

A smaller build can improve the installation and download experience.

## 12. Profile the Game

Use Unity's profiling tools to identify performance bottlenecks.

Monitor:

- CPU usage
- GPU usage
- Memory
- Rendering
- Physics
- Garbage collection

Optimize based on measured problems rather than assumptions.

## Mobile Optimization Checklist

- [ ] Tested on real devices
- [ ] Textures optimized
- [ ] Draw calls reviewed
- [ ] Models optimized
- [ ] Particle effects reviewed
- [ ] Physics optimized
- [ ] Audio compressed
- [ ] Memory usage checked
- [ ] UI optimized
- [ ] Asset loading reviewed
- [ ] Build size checked
- [ ] Profiler results reviewed

## Final Principle

Do not optimize only for the device used during development.

A mobile game template should be tested across the range of devices that the final game is expected to support.

## Further Reading

For a practical guide to optimizing Unity games for lower-end Android devices:

https://unitysourcecode.net/blog/optimize-a-unity-mobile-game-for-low-end-android-devices
