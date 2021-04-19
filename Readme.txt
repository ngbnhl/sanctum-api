Hiện tại api Sanctum em đang để là sử dụng API token

Trong trường hợp anh muốn sử dụng sang chế độ Cookie thì anh set up lại

1. Gỡ // ở mục 'stateful' trong file config/sanctum.php ( xóa luôn '' và gỡ) (bật chế độ stateful)
2. Chỉnh 'supports_credentials' => true trong file config/cors.php
3. Thay đổi tên schemes trong hàm loginWith('laravelSactum') ở component login.