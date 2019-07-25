vendor/illuminate/auth/EloquentUserProvider.php
validateCredentials


vendor/illuminate/hashing/BcryptHasher.php
check


vendor/illuminate/hashing/AbstractHasher.php
check

vendor/tymon/jwt-auth/src/JWTGuard.php
hasValidCredentials

tymon/jwt-auth/src/Providers/Auth/Illuminate.php
byCredentials


JWT调用顺序

JWTAuth->authenticate()

1、获取用户ID
$id = $this->getPayload()->get('sub');
2、JWTGuard->onceUsingId($id)
3、vendor/illuminate/auth/EloquentUserProvider.php retrieveById

