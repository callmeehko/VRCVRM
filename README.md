<div>
<img src="https://github.com/callmeehko/VRCVRM/blob/main/vrcvrmlogo.png?raw=true" height="128" style="display: flex; margin: auto;" />
<h2 style="text-align: center;">
VRCVRM - VRChat avatars as VTube avatars.
</h2>
</div>

**Note:** This does NOT use any code from VRChat, VRCFury, or any other proprietary software.

### Requirements
- A VRChat avatar with a Face Tracking Module (Jerry or EchoTheNeko)
- [VRCFaceTracking](https://docs.vrcft.io/ "VRCFaceTracking") (Use any Modules here, it supports just like VRChat's Client)
- Access to the Unity Editor (Unity 2022 via Creator Companion)
- [KlakNDI for Unity](https://github.com/keijiro/KlakNDI "KlakNDI for Unity")
- (Optional) Av3Emulator

### Features
- Video Output via NDI to OBS or any other capture software.
- Full VRChat Avatar Expressions
- Use Poiyomi shaders without getting hit by blinding amounts of purple. (those who know 💀)
- Robust SDK with a large amount of compatibility

### Why make this?
To be honest, I got bored one day and saw that no one had really tried this, primarily because it's kinda annoying to import VRChat avatars as VRM models into VSeeFace. This isn't supposed to be the BEST replacement, but it'll be a replacement that at least works.

### Setup
1. Setup a new VRChat 2022 Avatar Project (Reccomended) or use a pre-exisisting Avatar project.
2. Ensure your project has VRCFury enabled, and the face tracking module you'll be using.
3. Open `Window -> Package Manager` and click the + button, click `Install from tarball` and open your KlakNDI tar file.
4. Open `Window -> Package Manager` and click the + button, click `Install from Git` and paste in `https://github.com/CallMeEhko/VRCVRM.git`
5. Once installed, open `Window -> VRCVRM -> Setup` and go through the setup guide, this will setup the avatar for the expression parser, osc input detector, and any other things required.
6. Setup your enviroment, since this uses Unity, you can customize everything.
7. Go to `Window -> VRCVRM -> Control Panel` and drag your avatar from the Hiearchy to the Avatar box. Then click on `Start VTuber Enviroment`.
8. (Optional) Scroll down in the control panel to Video Output, drag the `VTube Camera` to the Video Output if you want to control what the output looks like.
9. Under Video Output, enable `Render NDI`, name your NDI Source what you want.
10. Head to the `Game` view and leave it open.
11. Add your NDI source to OBS or broadcast solution, it'll show up under the name you've put.
12. Profit on twitch.tv!

(PS, If you do end up using this... let me know! I wanna take a look at it from a viewer perspective!)

### Technical Insight
This really isn't that hard of a project to make, purely because you can just use NDI for video output, and make an osc server for VRCFT to connect to. A lot of the extra features just comes to making it function like VSeeFace or VTube Studio.

