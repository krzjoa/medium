<!-- #region -->
MAE = \frac{1}{N} \sum_{i = 1}^{N} |y_i - \hat{y}_i|

Q_q= \frac{1}{N} \sum_{i = 1}^{N} max(q(y_i - \hat{y}_i), (q-1)(y_i - \hat{y}_i))

MSE = \frac{1}{N} \sum_{i = 1}^{N} (y_i - \hat{y}_i)^{2}

Expectile_e= \frac{1}{N} \sum_{i = 1}^{N} w(y_i, \hat{y}_i)(y_i - \hat{y}_i)^2
\newline
where:
\newline
w(y_i, \hat{y}_i)   \left\{
    \begin{array}{l}
      1-e  \ for \ y_i < \hat{y}_i\\
      e    \ \ \ \ \ \ for \ y_i \geq \hat{y}_i
    \end{array}
  \right.
  
  
 
Expectile_e = \sum_{i=1}^{N}error(y_i, X_i, \beta)
\newline
where
\newline
\newline
error(y_i, X_i, \beta)  \left\{
    \begin{array}{l}
      (1-e)(y_i - X_i\beta)^2  \ for \ y_i < X_i\beta\\
      e(y_i - X_i\beta)^2       \ \ \ \ \ \ \ \ for \ y_i \geq X_i\beta
    \end{array}
  \right. 
  
 \frac{\partial error(y_i, X_i, \beta)}{\partial\beta}  \left\{
    \begin{array}{l}
      -2X_i\beta(1-e)(y_i - X_i\beta)  \ for \ y_i - X_i\beta\ < 0 \\
      -2X_i\beta e(y_i - X_i\beta)       \ \ \ \ \ \ \ \ for \ y_i - X_i\beta\  \geq 0
    \end{array}
  \right. 

<!-- #endregion -->
