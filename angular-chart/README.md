# AngularChart

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.1.1.

## Echarts installation
```
npm install echarts -S
npm install ngx-echarts -S
```

## Usage
Firstly, import NgxEchartsModule in your app module (or any other proper angular module):

```
import { NgxEchartsModule } from 'ngx-echarts';

@NgModule({
  imports: [
    NgxEchartsModule.forRoot({
      /**
       * This will import all modules from echarts.
       * If you only need custom modules,
       * please refer to [Custom Build] section.
       */
      echarts: () => import('echarts'), // or import('./path-to-my-custom-echarts')
    }),
  ],
})
export class AppModule {}
```