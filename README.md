# TBI Questionnaire App

# Simple questionnaire app to help identify the risk of a TBI having occurred in user and recommend action to the user based on results.

# Using Expo for deployment, commands to run since ethernet is not on the same subnet as WIFI, obviously use EXPO Go:

npx expo start --tunnel

# When finalizing build for IOS deployment, use EAS to avoid needing to use a Mac for packaging files for store:

# Install EAS CLI:

npm install -g eas-cli

# Configure Application for EAS:

eas build:configure

# Build for iOS "in the cloud":

eas build -p ios

# .ipa file should be produced at this point

# Submitting to the store (need Apple dev account at this point obviously):

eas submit -p ios
