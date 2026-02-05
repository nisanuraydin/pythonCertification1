test_settings = {
    'theme' : 'dark',
    'volume' : 'medium', 
    'notifications' : 'enabled'
}

def add_setting(settings, setting) :
    key, value = setting
    key = key.lower()
    value = value.lower()
    if key in settings :
        return f"Setting '{key}' already exists! Cannot add a new setting with this name."
    else :
        settings[key] = value
        return f"Setting '{key}' added with value '{value}' successfully!"
    return

def update_setting(settings, setting) :
    key, value = setting
    key = key.lower()
    value = value.lower()
    if key in settings :
        settings[key] = value
        return f"Setting '{key}' updated to '{value}' successfully!"
    else :
        return f"Setting '{key}' does not exist! Cannot update a non-existing setting."

def delete_setting(settings, key) :
    key = key.lower()
    if key in settings :
        settings.pop(key)
        return f"Setting '{key}' deleted successfully!"
    else :
        return "Setting not found!"
        
def view_settings(settings) :
    if len(settings) == 0 :
        return 'No settings available.'
    
    result = 'Current User Settings:'
    for key, value in settings.items() :
        result += f"\n{key.capitalize()}: {value}"

    result += "\n"
    return result

