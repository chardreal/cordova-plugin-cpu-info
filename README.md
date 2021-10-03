# Cordova CPU info plugin

Reads the CPU and some other hardware parameters of Android/iOS device

## Original author

Functionality of this plugin was created by Zhang Leo. This is NPM implementation of his [GitHub project](https://github.com/442623641/cordova-plugin-cpu-info) with few additions

## Install

	cordova plugin add cordova-clipboard

## Usage

Plugin creates `cordova.plugins.CPUInfo` object in global space. You can get the target info by call its methods

By Promise:

	cordova.plugins.CPUInfo.getMacAddress().then(function (address) {
		$('.address').text(address);
	});

Or with callback function:

	cordova.plugins.CPUInfo.getMacAddress(function (address) {
		alert(address);
	});

List of CPUInfo's methods:

### getMacAddress

Returns the mac address of the mobile 

### getCpuName

Returns the name of cpu

### getCurCpuFreq

Returns the current frequency of cpu 

### getMinCpuFreq

Returns the min frequency of cpu

### getMaxCpuFreq

Returns the max frequency of cpu

### getNumberCpuCores

Returns the number of cpu cores

### getRamTotalSize

Returns the total size of ram

### getRamAvailableSize

Returns the available size of ram

### getSDTotalSize

Returns the total size of sd

### getSDAvailableSize

Returns the available size of sd

### getRomTotalSize

Returns total size of rom

### getRomAvailableSize

Returns available size of rom

### getTimes

Returns the start time of the mobile
