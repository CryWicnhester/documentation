## Options

???+ info "Typescript typings"
    ```typescript
    /**
     * WidgetBot widget options
     */
    server: string                // Your guilds ID
    channel: string               // Channel ID
    options?: string              // WidgetBot widget options
    beta?: boolean                // Whether to use the beta domain or not
    buttons?: {                   // Change text of buttons
      primary?: string
      secondary?: string
    }
    username: string              // Use a specific username for the guest chatter

    /**
     * Aesthetic options
     */
    logo?: Url | 'intercom' | 'discord' | any | {
      url: Url
      size?: string
    }
    scheme?: 'dark' | 'light'     // Whether to show dark or light toasts
    style?: 'material' | 'discord'// Toggle button style
    colors?: {
      toggle?: string             // Crate toggle button color
      background?: string         // WidgetBot widget background
      button?: string             // WidgetBot `Start chatting` button color
    }
    position: {
      x: 'left' | 'right'
      y: 'top' | 'bottom'
    }
    contained: boolean            // Display modals in iframe or in the window

    /**
     * Notifications
     */
    notifications?: {
      indicator?: {
        enable: boolean
      }
      toasts?: {
        enable: boolean           // Whether to enable toasts or not
        visibilityTime?: number   // Max amount of time the toasts should be visible for (set to 0 to disable timeout)
        maxMessages?: number      // Max amount of messages to display on screen
        maxHeight?: string        // Max height of the toast container, CSS `calc()` can be used
      }
    }

    /**
     * General options
     */
    delay?: boolean               // Only load the widget once the button has been clicked
    ```