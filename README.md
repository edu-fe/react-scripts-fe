# react-scripts-fe

> 基于 react-scripts 定制



1.修改 package.json确定各版本
npm start -- >npm run dev

2，待研究

"bin": {
    "react-scripts-fe": "./bin/react-scripts.js"
  },

3 添加less

{
            test: /\.less/,
            use: [
              require.resolve('style-loader'),
              {
                loader: require.resolve('css-loader'),
                options: {
                  importLoaders: 1,
                },
              },
               {
                loader: require.resolve('less-loader')
              },
            ],
          },

 4 less全局变量