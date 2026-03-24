# jQuery Upgrade - Security Fix

## Changes Made

### 1. jQuery Version Upgrade
- **Old Version**: jQuery 2.4.1 (with known security vulnerabilities)
- **New Version**: jQuery 3.7.1 (latest stable 3.x release)
- **File**: `js/jquery.3.7.1.min.js`

### 2. Deprecated Method Fixes

#### options.js
- Replaced `.success()` with `.done()`
- Replaced `.error()` with `.fail()`

These methods were deprecated in jQuery 1.8 and removed in jQuery 3.0.

### 3. HTML Updates
- Updated `isitup.html` to reference `jquery.3.7.1.min.js`
- Updated `options.html` to reference `jquery.3.7.1.min.js`

### 4. Files Removed
- `js/jquery.2.4.1.min.js` (old vulnerable version)

## Testing Recommendations

1. Test the options page configuration loading from URL
2. Test file upload functionality
3. Test all health check endpoints
4. Verify notifications still work
5. Test badge toggle functionality
6. Verify build ID display

## Compatibility Notes

jQuery 3.x has better security, performance, and modern browser support. All deprecated methods have been updated to their modern equivalents.
