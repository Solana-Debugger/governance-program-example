# Solana Debugger: Governance program example

This is a snapshot of the SPL governance program, meant as an example program for the Solana Debugger.

The `debug_input` folder contains sample inputs that can be used to test the debugger.

The program includes a `save_input.rs` module which allows you to use integration tests to generate debugger inputs. For example, like this:

```
cd solana-program-library/governance/program

cargo-test-sbf test_create_realm --test process_create_realm -- --exact --nocapture

cargo-test-sbf test_refund_proposal_deposit --test process_refund_proposal_deposit -- --exact --nocapture
```

The generated inputs are stored in `solana-program-library/governance/program/debug_input`
