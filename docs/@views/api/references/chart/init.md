```typescript
(
  ds: string | HTMLElement,
  options?: {
    layout?: Array<{
      type: 'candle' | 'indicator' | 'xAxis'
      content?: Array<Indicator | string>
      options?: {
        id?: string
        height?: number
        minHeight?: number
        dragEnabled?: boolean
        order?: number
        state?: 'normal' | 'maximize' | 'minimize'
        axis?: {
          name?: string
          reverse?: boolean
          inside?: boolean
          position?: 'left' | 'right'
          scrollZoomEnabled?: boolean
          gap?: {
            top?: number
            bottom?: number
          }
        }
      }
    }>
    locale?: string
    styles?: string | Styles
    timezone?: string
    customApi?: {
      formatDate?: (timestamp: number, format: string, type: number) => string
      formatBigNumber?: (value: string | number) => string
    }
    thousandsSeparator?: {
      sign?: string
      format: (value: number | string) => string
    }
    decimalFold?: {
      threshold?: number
      format?: (value: number | string) => string
    }
  }
) => Chart
```