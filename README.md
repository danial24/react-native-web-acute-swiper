
## API

This plugin is forked from [react-native-web-plugin](https://www.npmjs.com/package/react-native-web-swiper).
You can find the docs for the available props from the link given above. There are three aditional props in this plugin

### **Additional Props**:

**scrollEnabled**(_boolean_): This will block the transition on swipe.

**showDots**(_boolean_): This will control the visibilty of bottom navigation dots View.

**showNextPrev**(_boolean_): There are next and prev buttons pre-rendered on the screen. You can control the visibility of those buttons with this prop.

## Usage

Here is a code snipet using all the above mentioned props:

    <Swiper
       scrollEnabled={false}
       ref={(c) => this._swiper = c}
       index={0}
       showDots={false}
       showNextPrev={false}
    >
       <ComponentOne moveNext={() => {
           //pass false tp move Next
           this._swiper.moveUpDown(false);
       }} />
       <ComponentTwo navigateBack={() => {
           //pass true to move back
           this._swiper.moveUpDown(true);
       }} />
    </Swiper>

## 🤝 Compatibility

| 🌏 Web | 🖥 Electron | 📱 React Native |
| :----: | :---------: | :-------------: |
|    ✅   |      ✅      |        ✅        |
