# vniolymp

Một gói LaTeX nhỏ, ổn định và tiện dụng để viết đề bài lập trình thi đấu. 

Gói này phụ thuộc nhiều vào trình dịch XeLaTeX, vì vậy hãy sử dụng trình dịch này nếu bạn dịch trên máy tính cá nhân, hoặc sử dụng Overleaf để đạt hiệu quả tốt nhất.

## Các tính năng chính

Viết đề bài trong kì thi trở nên dễ dàng, tiện lợi và đẹp:

```latex
% problem là môi trường để viết đề cho contest, có đánh số thứ tự, ghi mục lục, etc
\begin{problem}{A + B}{1s}{512 MiB}{stdin}{stdout}
Cho 2 số nguyên dương $a$ và $b$. Hãy tính tổng $a + b$.

\InputFile
Một dòng chứa 2 số nguyên dương $a$ và $b$.

\OutputFile
In ra $a + b$.

\Constraints
$1 \le a, b \le 10^9$.
\end{problem}
```

Đề bài cũng có thể được chèn vào sách, tài liệu rất nhanh gọn:
```latex
% statement là môi trường để viết đề bài gọn, dùng khi chèn vào sách, tài liệu
\begin{statement}{A + B}{1s}{512 MiB}{stdin}{stdout}
Cho 2 số nguyên dương $a$ và $b$. Hãy tính tổng $a + b$.

\InputFile
Một dòng chứa 2 số nguyên dương $a$ và $b$.

\OutputFile
In ra $a + b$.

\Constraints
$1 \le a, b \le 10^9$.
\end{statement}
```

Trong khi viết đề, nếu bạn muốn viết giới hạn, subtask, ví dụ, thì cũng rất đơn giản:

```latex
% Trong các môi trường viết đề ở trên, nếu bạn muốn thêm các thông tin khác cho đề bài, hãy thêm các macro này vào
\Explanations

Viết giải thích nếu có

\Scoring

Viết subtask nếu có

\Notes

Viết lưu ý nếu có

\Illustration

Minh hoạ nếu có
```
