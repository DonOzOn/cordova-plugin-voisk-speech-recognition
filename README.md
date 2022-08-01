cordova-plugin-voisk-speech-recognition
This codorva plugin offline speech recognition and speaker identification using Kaldi and Vosk libraries. use below function window.plugins.pocketsphinx.startListening(onRecognitionResult, onRecognitionError, options); window.plugins.pocketsphinx.stopListening();

startListening: function(successCallback, errorCallback, options) { options = options || {}; cordova.exec(successCallback, errorCallback, 'Pocketsphinx', 'startListening', []); },
 stopListening: function(successCallback, errorCallback) { cordova.exec(successCallback, errorCallback, 'Pocketsphinx', 'stopListening', []); }, 
 getSupportedLanguages: function(successCallback, errorCallback) { cordova.exec(successCallback, errorCallback, 'Pocketsphinx', 'getSupportedLanguages', []); }, 
 hasPermission: function(successCallback, errorCallback) { cordova.exec(successCallback, errorCallback, 'Pocketsphinx', 'hasPermission', []); }, 
 requestPermission: function(successCallback, errorCallback) { cordova.exec(successCallback, errorCallback, 'Pocketsphinx', 'requestPermission', []); }
