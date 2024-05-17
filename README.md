# floww-v2-general-custom-function

# README: Usage Examples for Alerts and Custom Popups

## 1. Toast Notification

### Displaying a Success Message
```javascript
showToast('Data saved successfully', 'success');
```

### Displaying an Error Message
```javascript
showToast('An error occurred', 'error');
```

### Displaying a Default Message
```javascript
showToast('Operation completed');
```

## 2. Custom Popup

### Displaying a Custom Confirmation Popup
```javascript
customFlowwShowCustomPopupconfirm(
  'deleteUser',     // Callback function name
  '123',            // Callback function argument(s)
  'Delete Item',    // Header text
  'Confirm',        // Button text
  'Are you sure?',  // Content text 1
  "This action can't be undone." // Content text 2
);
```

### Example Callback Function
```javascript
function deleteUser(userId) {
  console.log('User deleted:', userId);
}
```

### Example Usage
```javascript
customFlowwShowCustomPopupconfirm(
  'deleteUser', '123', 'Delete Item', 'Confirm', 'Are you sure?', "This action can't be undone."
);
```

Use these examples to integrate alerts and custom popups into your web pages quickly and efficiently.
