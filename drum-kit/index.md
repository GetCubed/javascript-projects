<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>Drum Kit</title>
        <link rel="stylesheet" href="style.css" />
        <script src="script.js" defer></script>
    </head>

    <body>
        <div class="keys">
            <div data-key="65" class="key">
                <kbd>A</kbd>
                <span class="sound">clap</span>
            </div>
            <div data-key="83" class="key">
                <kbd>S</kbd>
                <span class="sound">hihat</span>
            </div>
            <div data-key="68" class="key">
                <kbd>D</kbd>
                <span class="sound">kick</span>
            </div>
            <div data-key="70" class="key">
                <kbd>F</kbd>
                <span class="sound">openhat</span>
            </div>
            <div data-key="71" class="key">
                <kbd>G</kbd>
                <span class="sound">boom</span>
            </div>
            <div data-key="72" class="key">
                <kbd>H</kbd>
                <span class="sound">ride</span>
            </div>
            <div data-key="74" class="key">
                <kbd>J</kbd>
                <span class="sound">snare</span>
            </div>
            <div data-key="75" class="key">
                <kbd>K</kbd>
                <span class="sound">tom</span>
            </div>
            <div data-key="76" class="key">
                <kbd>L</kbd>
                <span class="sound">tink</span>
            </div>
        </div>

        <audio data-key="65" src="sounds/clap.wav"></audio>
        <audio data-key="83" src="sounds/hihat.wav"></audio>
        <audio data-key="68" src="sounds/kick.wav"></audio>
        <audio data-key="70" src="sounds/openhat.wav"></audio>
        <audio data-key="71" src="sounds/boom.wav"></audio>
        <audio data-key="72" src="sounds/ride.wav"></audio>
        <audio data-key="74" src="sounds/snare.wav"></audio>
        <audio data-key="75" src="sounds/tom.wav"></audio>
        <audio data-key="76" src="sounds/tink.wav"></audio>
    </body>

</html>