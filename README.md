CREATE TABLE `apply_member` (
    `apply_mem_id` int NOT NULL AUTO_INCREMENT COMMENT 'PK',
    `apply_id` int DEFAULT NULL COMMENT 'apply_id.apply (FK)',
    `mem_name` VARCHAR(20) DEFAULT NULL COMMENT '성명',
    `mem_officeph` VARCHAR(14) DEFAULT NULL COMMENT '전화 번호(사무실)',
    `phone` VARCHAR(14) DEFAULT NULL COMMENT '휴대폰번호',
    `mem_company` VARCHAR(50) DEFAULT NULL COMMENT '회사명(부서명)',
    `mem_position` VARCHAR(50) DEFAULT NULL COMMENT '직위',
    `mem_email` VARCHAR(50) DEFAULT NULL COMMENT '전자우편',
    `role` TINYINT DEFAULT NULL COMMENT '관리자종류: 1 = 총괄매니저 / 2 = 현장관리자',
    `mem_status` TINYINT DEFAULT 0 COMMENT '상태: 0=신청 / 1=거부 / 2=보류 / 3=승인',
    `created_at` VARCHAR(14) DEFAULT NULL,
	  `mem_id` int default NULL,
    PRIMARY KEY (`apply_mem_id`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8mb3;
